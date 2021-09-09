# Học Tailwind CSS

## Installation
Khởi tạo `package.json` với option `-y` để không bị hỏi bất kì câu hỏi nào

Note: Máy phải cài nodejs và npm rồi nhé

```js
npm init -y
npm install -D tailwindcss postcss autoprefixer vite
npx tailwindcss init -p
```
Để build tailwind ra file css với đường dẫn `build/tailwind.css` thì hãy chạy lệnh để build với file tailwind css tùy chỉnh
```
npx tailwindcss -i ./css/tailwind.css -o ./build/tailwind.css
```

Chạy lệnh này để build tất cả thuộc tính của tailwind. Tùy chọn `--watch` để thực hiện quy trình realtime nếu thay đổi CSS. Tùy chọn `--minify` để nén file CSS sẽ build ra

```
npx tailwindcss -o ./build/tailwind.css
```

Thêm scripts vào `packagist.json` để tiến hành tạo `dev` hoặc build CSS
```json
"scripts":
{
    "dev": "vite",
    "build:css": "npx tailwindcss -i ./css/tailwind.css -o ./build/tailwind.css --minify"
}
```

Chạy lệnh sau để run môi trường dev

```shell
npm run dev
```
Hoặc
```shell
yarn dev
```


