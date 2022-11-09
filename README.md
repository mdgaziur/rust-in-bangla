# রাস্ট দিয়ে প্রোগ্রামিং

রাস্ট হচ্ছে একটা মেমোরি সেইফ সিস্টেমস্ প্রোগ্রামিং ল্যাঙ্গুয়েজ।

সেইফ রাস্ট সব ধরনের মেমরি সংক্রান্ত বাগ যেমন: Out of bound read/write, Buffer overflow, Unsafe data race ইত্যাদি নির্মূল করে। এই ল্যাঙ্গুয়েজ একজন প্রো‌গ্রামারকে ভালো ও নিরাপদ সফটওয়্যার বানাতে সাহায্য করে। রাস্ট লো-লেভেল প্রোগ্রামিং করা অনেক সহজ করে দেয় এর মেমরি সেফটি দ্বারা। রাস্টের কম্পাইলার আপনার প্রোগ্রামের অনেক বাগ(যেগুলা অন্য সিস্টেমস্ প্রোগ্রামিং ল্যাঙ্গুয়েজ এর কম্পাইলার ধরতে পারে না) ধরে দিবে। যেমন, রিটার্ন টাইপ স্পেসিফাই করেও কোনো কিছু রিটার্ন না করলে রাস্ট কম্পাইলার এরর দিবে। আবার কোনো ভেক্টর এ ভুল ইন্ডেক্স থেকে কোনো আইটেম অ্যাক্সেস করলে রানটাইমে এরর দিবে। এখানে একটা বিষয় উল্লেখ্য যে সি এর `Segmentation Fault` কিন্তু এক্ষেত্রে সবসময় হয় না এবং অনেক সময় এটা মেমরি করাপ্ট করবে।

তবে রাস্ট কেবল সিস্টেমস্ প্রোগ্রামিং এর মধ্যেই সীমাবদ্ধ না। এর সিনট্যাক্স হাই লেভেল প্রোগ্রামিং ল্যাঙ্গুয়েজগুলোর মতো আর স্ট্যান্ডার্ড লাইব্রেরী অনেক রিচ বলে এটি দিয়ে কমান্ড লাইন অ্যাপ্লিকেশন, ওয়েব ডেভেলপমেন্ট, গুই ডেভেলপমেন্ট, গেম ডেভেলপমেন্টসহ অনেক ধরণের প্রোগ্রামিং খুব সহজেই করা যায়। রাস্ট এর আছে অফিসিয়াল প্যাকেজ রেজিষ্ট্রি [crates.io](https://crates.io) যেটাতে সব ধরনের প্রয়োজনীয় লাইব্রেরী পাওয়া যায়।

রাস্ট এমন এক ল্যাঙ্গুয়েজ যেটা স্কিলস্ এক ডোমেন থেকে আরেক ডোমেন এ ব্যবহার করা যায়। কেউ যদি ওয়েব ডেভেলপমেন্ট এর মাধ্যমে রাস্ট শিখে সে চাইলে পরে অর্জিত জ্ঞান ডেস্কটপ অ্যাপ্লিকেশন বানাতে প্রয়োগ করতে পারবে।[^১]

এই বইয়ে রাস্টের বেসিক সিনট্যাক্স এবং বিভিন্ন ফিচার নিয়ে কথা বলা হয়েছে। তাছাড়া এটাতে একটা কমান্ড লাইন অ্যাপ্লিকেশন এর মাধ্যমে এর বেশ কিছু ফিচার এর ব্যবহার দেখানো হয়েছে।

## নোট

[^১]: [এই অংশটি এখান থেকে নেয়া](https://doc.rust-lang.org/stable/book/foreword.html)
