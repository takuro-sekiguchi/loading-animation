# ローディングアニメーション

[デモサイトはこちら](https://taku-web3.com/project/loading-animation/index.html)

## ■新しく学んだこと
- ローディング中の線はspanで作れる
- display:flex; は親要素につける
- fancy-border-radiusでゆがみのborder-radiusを作れる
- load完了後のクラスを作っておいてJSで操作する
- JSでスタイルの中身を操作することもできる
- 書き方は1通りではないから自分なりの書き方を見つける


### fancy-border-radius
[border-radiusのゆがみを簡単に作れるサイト](https://9elements.github.io/fancy-border-radius/)

```js
    window.onload = () => {
      setTimeout(() => {
        const loader = document.querySelector('.loader');
        loader.classList.add('loaded');

        const content = document.querySelector('.content');
        //cssの中身を操作する方法
        content.style.display = 'block';
      }, 2000)
    }
```