# POSTER REPORT
For this project, I started by extracting the SVGs from the main poster, one by one. I made sure each SVG had the correct dimensions and that styles were set inline in the raw SVG code. This helped make sure they wouldn’t interfere with each other when putting everything together later.

I began the implementation by adding the background SVG first, then placing the illustrations on top of that, and finally positioning the text above all. I did all of this by visually aligning elements until everything looked right.

As I continued, I realized that raw SVG code takes up a lot of space in the HTML file. So, for the SVGs that I didn’t need to animate using SMIL, I moved them into a separate sprite.svg file. I then used the <use> tag in the HTML to fetch them. This helped keep the HTML cleaner and easier to work with.

## Elements and Animations
**Wi-Fi Signals:**
I animated the Wi-Fi signal waves to fade in and out, making it look like signals are being sent through the air. I used SMIL <animate> for this because it's simple for opacity animations.

**Pollution Smoke:**
The smoke from the factories is animated with both changing opacity and size. This gives the effect of live smoke that appears and disappears. I used CSS animation here which made it easy for chaining multiple animations like opacity and scale.

**Sun and Coin:**
I gave both the sun and the coin a swinging and floating effect using CSS animations. I chose CSS for these elements, this worked good, without needing to dig into the SVG structure.

**Earth’s Eyes:**
The Earth's eyes are animated to look from side to side using SMIL <animateTransform>. This gives the Earth a more lively, expressive, and even slightly helpless look, which adds a bit of personality and humor.

**Cloud Movement:**
Lastly, I animated a cloud to move along an infinity-shaped path using SMIL <animateMotion>. This made the cloud feel more dynamic and natural. I used SMIL motion animation here because it’s perfect for following custom paths.

## Conclusion
The final poster looks good and I feel I managed to make a solid copy of the original. It scales well from small to large screens, works in both Firefox and Chrome, and the print preview looked great. Overall, I’m happy with the result.