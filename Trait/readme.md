# Trait 
PHP-তে **Trait** হলো কোড পুনরায় ব্যবহার করার একটি উপায়, যা একাধিক ক্লাসে একই ফাংশনালিটি শেয়ার করতে দেয়। এটি ক্লাসের মতই, তবে ইনস্ট্যান্স করা যায় না এবং ইনহেরিটেন্স ছাড়াই বিভিন্ন ক্লাসে মেথড যুক্ত করতে ব্যবহার করা হয়।

**Trait উদাহরণ**:
```php
trait Logger {
    public function log($message) {
        echo $message;
    }
}

class User {
    use Logger;
}

$user = new User();
$user->log("Trait ব্যবহার করা হয়েছে!");
```

Trait এর মাধ্যমে কোড রিইউজ করা সহজ হয়, বিশেষ করে যখন একাধিক ক্লাসে একই মেথড ব্যবহার করতে হয়।