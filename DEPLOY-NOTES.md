# Hill Country Cleaning Co. - Location Pages Deployment Guide

## Files Included

1. **buda-house-cleaning.html** - Buda location page
2. **kyle-house-cleaning.html** - Kyle location page  
3. **south-austin-house-cleaning.html** - South Austin location page
4. **dripping-springs-house-cleaning.html** - Dripping Springs location page
5. **san-marcos-house-cleaning.html** - San Marcos location page
6. **cedar-park-house-cleaning.html** - Cedar Park location page
7. **privacy-policy.html** - Privacy policy page

## What's Optimized (AEO Elements)

Each location page includes:

- **LocalBusiness Schema** - Full structured data for Google/AI
- **FAQ Schema** - Structured FAQ data for AI citation
- **Semantic Intro** - First 100 words optimized for AI extraction
- **Location-specific keywords** - "[City] house cleaning" throughout
- **Meta descriptions** - Unique for each location
- **Canonical URLs** - Proper canonicalization

## How to Deploy to Netlify

### Option 1: Add to Existing Site (Recommended)

1. Go to your Netlify dashboard
2. Select your hillcountrycleaning.co site
3. Go to "Deploys" 
4. Drag and drop these files into your existing site folder

OR use Netlify CLI:
```bash
netlify deploy --prod
```

### Option 2: Manual File Structure

Your site structure should look like:
```
/
├── index.html (your main homepage)
├── buda-house-cleaning.html
├── kyle-house-cleaning.html
├── south-austin-house-cleaning.html
├── dripping-springs-house-cleaning.html
├── san-marcos-house-cleaning.html
├── cedar-park-house-cleaning.html
├── privacy-policy.html
└── llms.txt
```

### URL Structure After Deploy

- hillcountrycleaning.co/buda-house-cleaning
- hillcountrycleaning.co/kyle-house-cleaning
- hillcountrycleaning.co/south-austin-house-cleaning
- hillcountrycleaning.co/dripping-springs-house-cleaning
- hillcountrycleaning.co/san-marcos-house-cleaning
- hillcountrycleaning.co/cedar-park-house-cleaning
- hillcountrycleaning.co/privacy-policy

## Fixes for Main Site

Your current main site has two broken links:

1. **Email link** - Currently using CloudFlare email protection which isn't working
   - Change the footer email link from the encoded version to:
   - `<a href="mailto:jordan@hillcountrycleaning.co">Email Us</a>`

2. **Privacy Policy** - Currently links to "#" (does nothing)
   - Change to: `<a href="/privacy-policy">Privacy Policy</a>`

## After Deployment Checklist

- [ ] Verify all location pages load correctly
- [ ] Test all phone links work (click to call)
- [ ] Test all "Get a Quote" buttons link to Jobber
- [ ] Verify schema with Google's Rich Results Test
- [ ] Submit new URLs to Google Search Console
- [ ] Add location pages to your sitemap

## Schema Validation

Test your pages at:
- https://search.google.com/test/rich-results
- https://validator.schema.org/

Both should show LocalBusiness and FAQPage schema without errors.
