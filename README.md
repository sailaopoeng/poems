# WordPress to Hugo Migration (Hosted on AWS Amplify)

> ⚠️ **Note**: This project is **no longer in use**.  
> It has been moved into the [s3-static-portfolio](../s3-static-portfolio) repository under the branch **`poems`**.  
> This repo is kept for reference only.  

---

## 🚀 Process Overview  

1. **Export WordPress Content**  
   - From WordPress admin, export all posts/pages as an **XML file**.  

2. **Convert to Hugo**  
   - Use [wp2hugo](https://github.com/ashishb/wp2hugo) to transform the WordPress XML export into a Hugo-compatible project.  

3. **Fix Filename Issues**  
   - `wp2hugo` generates filenames that are too long due to URL-encoded Burmese titles.  
   - A **PowerShell script** was used to rename files into shorter, cleaner slugs.  

4. **Clean Post Content**  
   - Removed unnecessary metadata, formatting issues, and unused tags inside posts with PowerShell scripts.  

5. **Run Hugo**  
   - After cleanup, Hugo builds the static site successfully.  

6. **Deploy to AWS Amplify**  
   - The Hugo project is deployed to Amplify for fast, secure, and scalable hosting.  

---

## 🛠 Tools & Scripts  

- **wp2hugo** → WordPress XML → Hugo project.  
- **PowerShell scripts** → Automate filename shortening and post cleanup.  
- **Hugo** → Static site generator.  
- **AWS Amplify** → Hosting platform.  

---

## 🔗 References  

- [Hugo Documentation](https://gohugo.io/documentation/)  
- [wp2hugo](https://github.com/ashishb/wp2hugo)  
- [AWS Amplify Hosting](https://docs.amplify.aws/hosting/)  
