# 🚀 GitHub Deployment Guide

## Step 1: Create a New GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Enter repository name: `food-ordering-dashboard`
3. Add description: "Executive Power BI Dashboard for Food Ordering & Customer Behavior Analytics"
4. Choose **Public** visibility (recommended for portfolio)
5. Do NOT initialize with README (we already have one)
6. Click **Create repository**

## Step 2: Push Local Repository to GitHub

### Option A: HTTPS
```bash
cd food-ordering-dashboard
git remote add origin https://github.com/YOUR_USERNAME/food-ordering-dashboard.git
git branch -M main
git push -u origin main
```

### Option B: SSH (Recommended)
```bash
cd food-ordering-dashboard
git remote add origin git@github.com:YOUR_USERNAME/food-ordering-dashboard.git
git branch -M main
git push -u origin main
```

### Option C: GitHub CLI
```bash
cd food-ordering-dashboard
gh repo create food-ordering-dashboard --public --source=. --push
```

## Step 3: Verify Deployment

After pushing, your repository should look like this:

```
food-ordering-dashboard/
├── README.md              ✅ Professional documentation
├── LICENSE                ✅ MIT License
├── .gitignore             ✅ Clean repo rules
├── data/                  ✅ 3 CSV datasets
│   ├── food_orders_data.csv
│   ├── customers_data.csv
│   └── restaurants_data.csv
├── dax/                   ✅ 45 DAX measures
│   └── DAX_Measures_Complete.txt
├── images/                ✅ Dashboard previews
│   ├── dashboard-light.png
│   └── dashboard-dark.png
├── docs/                  ✅ Implementation guide
│   └── PowerBI_Implementation_Guide.txt
└── powerbi/               ✅ Theme files
    ├── theme-light.json
    └── theme-dark.json
```

## Step 4: Enable GitHub Features

### GitHub Pages (Optional - for portfolio)
1. Go to **Settings** → **Pages**
2. Source: Deploy from a branch
3. Branch: `main` / `root`
4. Your dashboard will be live at: `https://YOUR_USERNAME.github.io/food-ordering-dashboard/`

### GitHub Topics (for discoverability)
Add these topics to your repository:
- `powerbi`
- `dax`
- `data-analytics`
- `foodtech`
- `business-intelligence`
- `dashboard`
- `data-visualization`
- `microsoft`
- `sql`
- `portfolio`

### Social Preview
1. Go to **Settings** → **Social preview**
2. Upload `images/dashboard-light.png` as the social card
3. This image will appear when sharing on LinkedIn/Twitter

## Step 5: Update README Links

After deployment, update these links in `README.md`:

```markdown
[![Live Demo](https://img.shields.io/badge/Live%20Demo-View%20Dashboard-2563EB?style=for-the-badge)](https://YOUR_USERNAME.github.io/food-ordering-dashboard/)
```

## Step 6: Share Your Portfolio

### LinkedIn Post Template
```
🚀 Just published my Executive Power BI Dashboard for FoodTech Analytics!

Built a complete BI solution with:
✅ 5,000 real-world order records
✅ 45 DAX measures (RFM, CLV, NPS)
✅ Star schema data model
✅ Light & Dark themes
✅ 10 interactive slicers

Tech Stack: Power BI | DAX | Data Modeling | UX Design

🔗 GitHub: github.com/YOUR_USERNAME/food-ordering-dashboard

#PowerBI #DataAnalytics #BusinessIntelligence #FoodTech #Portfolio
```

### Resume Bullet Points
- **Designed and deployed** an executive-level Power BI dashboard analyzing 5,000+ food orders across 8 cities, delivering actionable insights to C-suite stakeholders
- **Engineered 45 DAX measures** including RFM segmentation, Customer Lifetime Value, and Net Promoter Score for advanced customer analytics
- **Architected a star schema data model** with 3 dimension tables and 1 fact table, optimizing query performance for real-time decision-making
- **Implemented dual-theme UX** (light/dark) with conditional formatting, cross-filtering, and 10 interactive slicers for self-service analytics

---

## 📋 Pre-Deployment Checklist

- [ ] GitHub account created
- [ ] Repository name set to `food-ordering-dashboard`
- [ ] Local repo pushed to GitHub
- [ ] README.md displays correctly
- [ ] Images render in README
- [ ] GitHub topics added
- [ ] Social preview image uploaded
- [ ] LinkedIn post drafted
- [ ] Resume updated with project details

---

## 🆘 Troubleshooting

### "Permission denied" when pushing
```bash
git remote set-url origin https://YOUR_TOKEN@github.com/YOUR_USERNAME/food-ordering-dashboard.git
```

### Large file issues
```bash
git lfs track "*.csv"
git add .gitattributes
git commit -m "Track CSV files with Git LFS"
```

### Merge conflicts
```bash
git pull origin main --rebase
git push origin main
```

---

**Ready to deploy! 🚀**
