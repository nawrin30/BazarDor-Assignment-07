# বাজার দর (BazarDor)

**বাজার দর (BazarDor)** হলো একটি responsive বাংলা ওয়েব অ্যাপ, যেখানে বাংলাদেশের নিত্যপ্রয়োজনীয় পণ্যের সম্ভাব্য দাম দেখা এবং বিভিন্ন বাজারের দামের তুলনা করা যায়।

## Technologies Used

- Next.js App Router
- React (JavaScript / JSX)
- CSS for responsive styling
- Better Auth for authentication and profile updates
- SQLite (`better-sqlite3`) for local authentication data
- REST API for product and category data
- Lucide React icons
- React Hot Toast notifications

## 5 Key Features

1. **বাংলা ও responsive interface:** মোবাইল, ট্যাবলেট ও ডেস্কটপে ব্যবহারযোগ্য নেভিগেশন, হিরো সেকশন এবং তারিখ প্রদর্শন।
2. **পণ্য ও ক্যাটাগরি ব্রাউজিং:** চাল, ডাল, তেল, সবজি, মাছ, মাংসসহ বিভিন্ন ক্যাটাগরির পণ্য দেখা।
3. **বাজারভিত্তিক দাম তুলনা:** পণ্যের বিস্তারিত পেজে বিভিন্ন বাজারের দাম এবং সর্বনিম্ন/সর্বোচ্চ দামের তথ্য।
4. **দাম অনুযায়ী sorting:** ডিফল্ট, দাম কম থেকে বেশি এবং দাম বেশি থেকে কম; বাংলা অঙ্ক থাকলেও সংখ্যামূল্য অনুযায়ী সাজানো হয়।
5. **Authentication ও profile management:** Better Auth দিয়ে sign up/sign in, protected profile এবং আলাদা route থেকে নাম আপডেট।

## API

- Primary: `https://api.api-store.workers.dev/api/bazardor`
- Alternative: `https://api.abcz.workers.dev/api/bazardor`

API দুটোই unavailable হলে local sample data ব্যবহার করা হয়। Sample data live market data নয়।

## Local Setup

1. Node.js LTS ইনস্টল করুন (Node.js 22.5+ recommended)।
2. Dependencies ইনস্টল করুন:

   ```bash
   npm install
   ```

3. `.env.example` থেকে `.env` তৈরি করে `BETTER_AUTH_SECRET` এবং `BETTER_AUTH_URL` সেট করুন।
4. Development server চালান:

   ```bash
   npm run dev
   ```

5. `http://localhost:3000` খুলুন।

Google/GitHub sign-in ব্যবহার করতে চাইলে `.env`-এ সংশ্লিষ্ট OAuth credentials সেট করতে হবে। Local SQLite database ব্যবহার করায় deployment-এর ক্ষেত্রে persistent storage নিশ্চিত করুন।

## Submission Links

- Live Link: _deployment-এর পর যোগ করুন_
- GitHub Repository: _repository push করার পর যোগ করুন_
