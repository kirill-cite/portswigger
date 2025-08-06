# Lab 01: Limit overrun race conditions

## Lab's purchasing flow contains a race condition

### Credentials - wiener:peter

1. Login with credentials wiener:peter

2. Add item to the cart and apply promo

3. Look at actions in Burp

4. Try to send requests with and without cookie

5. To trigger race conditions create Custom actions (Trigger race condition)

6. Solutions:

-Send POST /cart/coupon HTTP/2 request multiple times to get low price

-Create group of equal requests and send it parallel (HTTP/2)

-We can make PoC using Intruder with null payload
