<img src="https://res.cloudinary.com/dbjrx698c/image/upload/v1704611347/logo_w4vxp0.png" width="100" height="100" style="display: block; margin: 0 auto;">

# Next Rating Component
I've been searching for a reliable React rating component for Next.js with server-side rendering (SSR) support and essential features like fractional ratings. After trying several existing libraries over the past five days, I've found that many either don't work well with SSR, lack crucial functionality, or don't support fractions. Therefore, I've decided to build my own customizable rating component in TypeScript to meet common project needs.

<a href="https://www.buymeacoffee.com/siamahnaf" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

- Small in Size
- Zero Dependency
- Fractional step (It support any fractional value)
- Custom Icon
- All necessary options

# Demo
See <a href="">Live Demo</a>

# Installation

```bash
$ npm i next-rating-component
```

# App Router
```javascript
"use client"
import { useState } from "react";
import { Rating } from "next-rating-component";

const MyComponent = () => {
    const [rating, setRating] = useState<number>(0);


    return (
        <div>
            <Rating
                value={rating}
                onChange={(e) => setRating(e)}
                fractions={0.1}
            />
        </div>
    );
};

export default MyComponent;
```

# Available props

<table width="100%">
  <tr>
    <th> Name </th>
    <th> Description </th>
    <th> Type </th>
    <th> Default/Required </th>
  </tr>
  <tr>
    <td> maxRating </td>
    <td> Rating star count </td>
    <td> number </td>
    <td> 5 </td>
  </tr>
   <tr>
    <td> value </td>
    <td> The value of rating (You can use Rating component with controls using this value prop) </td>
     <td> number </td>
    <td> Required </td>
  </tr>
   <tr>
    <td> icon </td>
    <td> Change the icon of Rating Component (Only SVG Icon supported) </td>
     <td> React Element </td>
    <td> Optional </td>
  </tr>
   <tr>
    <td> fractions </td>
    <td> Fractional Step For Icon </td>
     <td> number </td>
    <td> 1 </td>
  </tr>
  <tr>
    <td> onChange </td>
    <td> The new rating value when clicked </td>
     <td> (newRating)=> void </td>
    <td> Optional </td>
  </tr>
   <tr>
    <td> onHover </td>
    <td> The new rating value when hovered </td>
     <td> (newRating)=> void </td>
    <td> ease </td>
  </tr>
  <tr>
    <td> readOnly </td>
    <td> The interactivity of the icon </td>
     <td> boolean </td>
    <td> false </td>
  </tr>
  <tr>
    <td> Size </td>
    <td> The Size of the Icon </td>
     <td> number </td>
    <td> 24 </td>
  </tr>
  <tr>
    <td> emptyColor </td>
    <td> The color of the empty Icon </td>
     <td> string </td>
    <td> #dfe2e6 </td>
  </tr>
   <tr>
    <td> fillColor </td>
    <td> The color of the fill Icon </td>
     <td> string </td>
    <td> #fab005 </td>
  </tr>
  <tr>
    <td> toolTip </td>
    <td> For showing tooltip </td>
     <td> boolean </td>
    <td> false </td>
  </tr>
  <tr>
    <td> customTooltip </td>
    <td> Custom tooltip for every step. Here step will 2 decimal position number for each step </td>
     <td> {step:number, text:string}[] </td>
    <td> optional </td>
  </tr>
</table>

# Stay in touch

- Author - [Siam Ahnaf](https://www.siamahnaf.com/)
- Website - [https://www.siamahnaf.com/](https://www.siamahnaf.com/)
- Twitter - [https://twitter.com/siamahnaf198](https://twitter.com/siamahnaf198)
- Github - [https://github.com/siamahnaf](https://github.com/siamahnaf)