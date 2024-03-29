# রাস্ট প্রোগ্রাম এর গঠন

আমরা আগের `Hello World` প্রোগ্রামে ফিরে যাই:

```rust
fn main() {
    println!("Hello World!");
}
```

আগেই বলেছিলাম যে আমরা একটা "বাইনারি" প্রোগ্রাম বানিয়েছিলাম। তো, `C` আর `C++‍` এর মতো রাস্টের বাইনারিতে `main` ফাংশন থেকে কোড
রান করা শুরু হয়। তবে, ওই ল্যাঙ্গুয়েজগুলোর মতো এখানে Command line argument নিতে ফাংশনে কোনো আর্গুমেন্ট নিতে হয় না। Command line
arguments নিয়ে পরে বিস্তারিত জানবো আমরা।

এখন, এই ফাংশনে আমরা আমাদের ইচ্ছামতো কোড লিখতে পারি। যেমন, আমরা চাইলে দুটি সংখ্যা যোগ করে দেখাতে পারি:

```rust
fn main() {
    println!("2 + 2 = {}", 2 + 2);
}
```

আমরা `println!` কে একটি ফরম্যাট স্ট্রিং পাঠিয়েছি আর `{}` দিয়ে দেখিয়েছি কোথায় আমাদের আউটপুট দেখাতে হবে।

এখন, প্রত্যেকটা ফাংশনের বডিতে এক বা একাধিক `Expression` আর `Statement` থাকতে পারে। Expression হচ্ছে সেইসব কোড যেগুলা থেকে
কোনো মান পাওয়া যায়। আর statement হলো সেইসব কোড যেগুলো থেকে কোনো মান পাওয়া যায় না। যেমন: `1 + 2` একটি expression এবং
‍`return 1` হচ্ছে একটি ‍statement। কারণ, `1 + 2` থেকে আমরা `3` কে পাই। কিন্তু `return 1` আমাদেরকে `()` দেয়। এখন, বিশেষ কিছু
ক্ষেত্র ছাড়া সবসময় expression এর পরে সেমিকোলন `;` দিতে হয়। পরের অংশে আমরা এটা নিয়ে বিস্তারিত জানবো।