# Button
Button의 normal, positive, negative 상태에서 hover, active일 때 변화가 있게 만들기
(:root 사용)
<!DOCTYPE html>
<html lang="ko-KR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>수업실습 : BUTTON</title>
    <style>
      :root {
        --main-background-color: #343f50;
        --positive-color: #439aff;
        --negative-color: #eb5757;
        --text-color-hover: #fff;
        --normal-border-color: #1a202c;
        --shadow-color-hover: #rgba(255, 255, 25, , 0.2);
        --shadow-color-active: #rgba(0, 0, 0, 0.2);
      }

      button {
        width: 88px;
        height: 32px;
        box-shadow: rgba(255, 255, 255, 0.1);
        font-size: 12px;
        text-align: center;
        font-weight: 700;
        line-height: 0.9;
      }

      .normal {
        color: #cbd5df;
        background-color: var(--main-background-color);
        border-color: var(--normal-border-color);
      }

      .normal:hover {
        color: var(--text-color-hover);
        background-color: var(--main-background-color);
        box-shadow: var(--shadow-color-hover);
        border-color: var(--normal-border-color);
        text-decoration: underline;
      }

      .normal:active {
        color: var(--text-color-hover);
        background-color: var(--main-background-color);
        box-shadow: var(--shadow-color-active);
        border-color: var(--normal-border-color);
        text-decoration: underline;
      }

      /* .normal:disabled {
        color: #4a5568;
        background-color: var(--main-background-color);
      } */

      .positive {
        color: var(--positive-color);
        background-color: var(--main-background-color);
      }

      .positive:hover {
        color: var(--text-color-hover);
        background-color: var(--positive-color);
        border-color: var(--positive-color);
        box-shadow: var(--shadow-color-hover);
        text-decoration: underline;
      }

      .positive:active {
        color: var(--text-color-hover);
        background-color: var(--positive-color);
        border-color: var(--positive-color);
        box-shadow: var(--shadow-color-active);
        text-decoration: underline;
      }

      .negative {
        color: var(--negative-color);
        background-color: var(--main-background-color);
      }

      .negative:hover {
        color: var(--text-color-hover);
        background-color: var(--negative-color);
        border-color: var(--negative-color);
        box-shadow: var(--shadow-color-hover);
        text-decoration: underline;
      }

      .negative:active {
        color: var(--text-color-hover);
        background-color: var(--negative-color);
        border-color: var(--negative-color);
        box-shadow: var(--shadow-color-active);
        text-decoration: underline;
      }

      .disabled {
        color: #4a5568;
        background-color: var(--main-background-color);
      }
    </style>
  </head>
  <body>
    <button class="normal">Button</button>
    <button class="positive">Yes</button>
    <button class="negative">Del</button>
    <!-- <button class="disable">Button</button> -->
    <button type="button" class="disabled" disabled>Button</button>
  </body>
</html>
