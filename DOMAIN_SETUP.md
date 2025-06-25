# Sronic.com Domain Setup Guide

## 🎯 Current Status
✅ **GitHub Pages Repository**: `https://github.com/sronicplatform/sronic.github.io.git`  
✅ **CNAME File**: Created and pushed to repository  
✅ **Website Files**: All HTML, CSS, and JS files are ready  

## 🔧 Squarespace Domain Configuration

### Step 1: Access Squarespace Domain Settings
1. Log into your Squarespace account
2. Go to **Settings** → **Domains**
3. Find your `sronic.com` domain
4. Click on **DNS Settings** or **Advanced DNS Settings**

### Step 2: Configure DNS Records
You need to add/update these DNS records in Squarespace:

#### A Records (for root domain)
```
Type: A
Name: @ (or leave blank)
Value: 185.199.108.153
TTL: 3600 (or default)

Type: A
Name: @ (or leave blank)
Value: 185.199.109.153
TTL: 3600 (or default)

Type: A
Name: @ (or leave blank)
Value: 185.199.110.153
TTL: 3600 (or default)

Type: A
Name: @ (or leave blank)
Value: 185.199.111.153
TTL: 3600 (or default)
```

#### CNAME Record (for www subdomain)
```
Type: CNAME
Name: www
Value: sronicplatform.github.io
TTL: 3600 (or default)
```

### Step 3: Remove/Disable Squarespace Site
1. In Squarespace, go to **Settings** → **Domains**
2. If there's a Squarespace site connected to sronic.com, disconnect it
3. Make sure the domain is not pointing to a Squarespace site

### Step 4: Configure GitHub Pages
1. Go to your GitHub repository: `https://github.com/sronicplatform/sronic.github.io`
2. Click **Settings** tab
3. Scroll down to **Pages** section (left sidebar)
4. Under **Custom domain**, enter: `sronic.com`
5. ✅ Check **Enforce HTTPS**
6. Click **Save**

## ⏱️ DNS Propagation Time
- **Typical time**: 24-48 hours
- **Sometimes faster**: 2-4 hours
- **Check status**: Use `dig sronic.com` or online DNS checkers

## 🔍 Testing Your Setup

### Check DNS Propagation
```bash
# Check A records
dig sronic.com A

# Check CNAME record
dig www.sronic.com CNAME

# Check GitHub Pages status
curl -I https://sronic.com
```

### Expected Results
- `sronic.com` should resolve to GitHub Pages IP addresses
- `www.sronic.com` should redirect to `sronic.com`
- HTTPS should work automatically

## 🚨 Troubleshooting

### Common Issues

**1. Domain Not Working After 24 Hours**
- Double-check DNS records in Squarespace
- Verify GitHub Pages custom domain is set
- Contact Squarespace support if needed

**2. HTTPS Not Working**
- Ensure "Enforce HTTPS" is checked in GitHub Pages
- Wait for SSL certificate to be issued (can take up to 24 hours)

**3. www Subdomain Not Working**
- Verify CNAME record points to `sronicplatform.github.io`
- Check that GitHub Pages is enabled

**4. Mixed Content Errors**
- Ensure all internal links use HTTPS
- Check that external resources use HTTPS

### Squarespace-Specific Issues

**If Squarespace Won't Let You Edit DNS:**
1. Contact Squarespace support
2. Request DNS management access
3. Or transfer domain to another provider (Namecheap, GoDaddy, etc.)

**If Domain is Locked to Squarespace Site:**
1. Disconnect domain from Squarespace site first
2. Then configure DNS records
3. May need to contact support

## 📞 Support Contacts

- **Squarespace Support**: Available in your Squarespace dashboard
- **GitHub Support**: https://support.github.com
- **DNS Checker**: https://www.whatsmydns.net

## ✅ Success Checklist

- [ ] DNS A records configured in Squarespace
- [ ] DNS CNAME record configured in Squarespace
- [ ] Custom domain set in GitHub Pages
- [ ] HTTPS enforced in GitHub Pages
- [ ] Domain propagates correctly (check after 24 hours)
- [ ] Website loads at https://sronic.com
- [ ] www.sronic.com redirects to sronic.com

## 🎉 Once Complete

Your website will be accessible at:
- **Primary**: https://sronic.com
- **Redirect**: https://www.sronic.com → https://sronic.com
- **GitHub Pages**: https://sronicplatform.github.io (fallback)

**Your Sronic website will be live on your custom domain! 🌍** 