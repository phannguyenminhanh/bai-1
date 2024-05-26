Cả for...of và for...in đều là các cấu trúc vòng lặp trong JavaScript, nhưng chúng có mục đích và cách hoạt động khác nhau. Dưới đây là sự khác biệt giữa chúng và một ví dụ minh họa:

for...of:
Vòng lặp for...of được sử dụng để lặp qua các giá trị của một đối tượng có thể lặp được như mảng, chuỗi, Set, Map, NodeList, v.v.

javascript
Copy code
const array = [1, 2, 3, 4, 5];
for (const element of array) {
console.log(element);
}
Trong ví dụ trên, for...of lặp qua từng phần tử trong mảng array, và biến element sẽ nhận giá trị của từng phần tử trong mảng.

for...in:
for...in được sử dụng để lặp qua các thuộc tính của một đối tượng có thể đếm được như một object, một mảng (dùng để lặp qua các chỉ số của mảng), hoặc các loại đối tượng có thể đếm được khác.

javascript
Copy code
const person = {
name: "John",
age: 30,
city: "New York"
};
for (const key in person) {
console.log(key + ": " + person[key]);
}
Trong ví dụ này, for...in lặp qua các thuộc tính của đối tượng person, và biến key sẽ nhận tên của từng thuộc tính. Để truy cập vào giá trị của thuộc tính, chúng ta sử dụng person[key].

Sự khác biệt:
for...of được sử dụng để lặp qua các phần tử của một cấu trúc dữ liệu có thứ tự như mảng, trong khi for...in được sử dụng để lặp qua các thuộc tính của một đối tượng.
Trong for...of, biến lặp được gán giá trị của từng phần tử trong cấu trúc dữ liệu, trong khi trong for...in, biến lặp được gán tên của từng thuộc tính của đối tượng.
