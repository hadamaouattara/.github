# 🚀 Universal GitHub Actions - Quick Start Guide

## ⚡ 30-Second Setup

### Option 1: One-Click Installation (Recommended)

1. **Go to your project** on GitHub
2. Click **Actions** tab
3. Click **"New workflow"**
4. Search **"Setup Universal Automation"**
5. Click **"Configure"** → **"Start commit"**
6. **Run the workflow**: Actions → Setup Universal Automation → Run workflow

### Option 2: Command Line (Advanced)

```bash
# In your project directory
curl -o .github/workflows/setup-automation.yml \
  https://raw.githubusercontent.com/hadamaouattara/.github/main/workflow-templates/setup-universal-automation.yml

# Commit and push
git add .github/workflows/setup-automation.yml
git commit -m "🚀 Add Universal Automation Setup"
git push

# Then run via GitHub UI: Actions → Setup Universal Automation → Run workflow
```

## 🎯 What You Get Immediately

### ✅ Quality Gate (Every commit)
- Framework detection (Next.js, React, Vue, etc.)
- Build validation
- Security scan
- Code quality checks

### ✅ Health Monitor (Every 6 hours)
- Post-deployment validation
- Performance checks
- Uptime monitoring
- Issue detection

### ✅ Auto Rollback (Emergency response)
- Automatic failure detection
- Smart rollback to last stable version
- Zero-downtime recovery
- Incident documentation

### ✅ Performance Audit (Daily)
- Lighthouse scoring
- Bundle analysis
- Dependency monitoring
- Optimization recommendations

## 🛠️ Configuration Options

When running the setup workflow, choose:

- **`all`** → Complete automation suite (recommended)
- **`minimal`** → Quality Gate + Health Monitor only
- **Individual workflows** → Pick specific tools

## 📊 Expected Results

After setup, you'll see:
- **✅ Green checkmarks** on all commits
- **🔍 Detailed reports** in Actions tab
- **📈 Performance insights** in daily audits
- **🛡️ Zero failed deployments** reaching production

## 🆘 Troubleshooting

**Issue**: Workflow fails on first run
**Solution**: Ensure `package.json` has required scripts:
```json
{
  "scripts": {
    "build": "next build", // or your build command
    "lint": "next lint"    // optional but recommended
  }
}
```

**Issue**: Build takes too long
**Solution**: The system auto-detects and optimizes for your framework

**Issue**: Need custom configuration
**Solution**: Edit workflows in `.github/workflows/` after installation

## 📞 Support

- 📚 **Full docs**: [README.md](README.md)
- 🐛 **Issues**: Create issue mentioning @hadamaouattara
- 💬 **Questions**: Check the Actions logs first

---

**🎯 Result**: Production-ready automation in under 2 minutes!
