# BadApple on GPKI Dialog
![image](https://user-images.githubusercontent.com/27724108/114796622-6945bf80-9dcc-11eb-9444-7743dec2d387.png)

You know that GPKI sucks right?  
Yes, me either. Let's make it better by playing Bad Apple on it.

## Demonstration
<img width="1029" alt="image" src="https://user-images.githubusercontent.com/27724108/114867058-4a2c4980-9e2f-11eb-8f01-5cda2f3fbad4.png"><br>
Yes, You've seen it. Bad Apple Running on <a href="https://gov.kr">South Korean Government Portal (정부24)</a>. <strike>very funny isn't it</strike>  

[Buggy Demo available at here (YouTube)](https://www.youtube.com/watch?v=Z6ZeLVP_nHY)

## GitHub Actions Status

| Name                      | Status                                                                                                         |
|---------------------------|----------------------------------------------------------------------------------------------------------------|
| ESLint                    | ![ESLint](https://github.com/Alex4386/badapple-gpki-dialog/workflows/ESLint/badge.svg)                         |

## How to install
1. Install graphicsmagick
2. Install ffmpeg
3. Download badapple youtube video, which I won't do it for you.  
   Because Copyright / Licensing issues.
4. Download it I don't care how you donwnload it. and place it on root directory. rename the file as `footage.mp4`
5. run `ffmpeg -i footage.mp4 -vf fps=24 image/%05d.png` on output directory
6. Run server via `yarn start`
7. open up [gov.kr](https://gov.kr) and try to login, when the GPKI popup opens, open developer tools. (disable breakpoints if necessary)
8. copy the contents of `browser.js`
9. paste it into console.
10. run code via typing `start()`.

## License
[WTFPL](LICENSE)
