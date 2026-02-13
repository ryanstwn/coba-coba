# 🚀 Quick Start Guide

## Langkah Cepat Menjalankan Project

### Option 1: Run Dashboard Locally (Recommended untuk Testing)

```bash
# 1. Clone repository
git clone https://github.com/USERNAME/bike-sharing-analysis.git
cd bike-sharing-analysis

# 2. Create virtual environment (optional tapi recommended)
python -m venv venv

# Activate virtual environment
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run dashboard
streamlit run dashboard.py

# Dashboard akan terbuka di browser pada http://localhost:8501
```

### Option 2: Run Jupyter Notebook

```bash
# 1. Install Jupyter (jika belum)
pip install jupyter

# 2. Run Jupyter
jupyter notebook

# 3. Buka file: bike_sharing_analysis.ipynb

# 4. Run All Cells (Cell > Run All)
```

### Option 3: Access Deployed Dashboard

Langsung akses dashboard yang sudah deployed:
- URL: `https://your-deployed-dashboard-url.streamlit.app`

## 📝 File Structure

```
bike-sharing-analysis/
│
├── 📊 hour.csv                        # Dataset asli
├── 📓 bike_sharing_analysis.ipynb     # Analisis lengkap
├── 🎨 dashboard.py                    # Dashboard Streamlit
├── 📦 requirements.txt                # Dependencies Python
├── 📖 README.md                       # Dokumentasi utama
├── 🚀 DEPLOYMENT_GUIDE.md            # Panduan deployment
├── ⚡ QUICKSTART.md                   # File ini
└── 🚫 .gitignore                      # Git ignore rules
```

## ✅ Checklist Pre-submission

Sebelum submit, pastikan:

1. **Local Testing**
   - [ ] Dashboard berjalan lancar di local
   - [ ] Semua tab dapat diakses
   - [ ] Filter bekerja dengan baik
   - [ ] Tidak ada error di console

2. **GitHub**
   - [ ] Repository public
   - [ ] Semua file sudah di-push
   - [ ] README lengkap dan jelas
   - [ ] Notebook sudah dijalankan (show outputs)

3. **Deployment**
   - [ ] Dashboard deployed ke Streamlit Cloud
   - [ ] URL dapat diakses publik
   - [ ] Dashboard load dengan baik (< 5 detik)
   - [ ] Tidak ada error 500

4. **Video**
   - [ ] Video duration 5-7 menit
   - [ ] Audio clear
   - [ ] Demonstrasi semua features
   - [ ] Upload ke YouTube (public/unlisted)
   - [ ] Include links di description

## 🔧 Troubleshooting Common Issues

### Issue: ModuleNotFoundError

**Solution:**
```bash
pip install -r requirements.txt --upgrade
```

### Issue: FileNotFoundError: 'hour.csv'

**Solution:**
Pastikan `hour.csv` ada di directory yang sama dengan `dashboard.py`
```bash
# Check current directory
pwd
# List files
ls -la
# If hour.csv not found, download again
```

### Issue: Dashboard sangat lambat

**Solution:**
```python
# Dashboard.py sudah menggunakan @st.cache_data
# Tapi jika masih lambat, coba:
# 1. Reduce data size dengan sampling
# 2. Filter data range yang lebih kecil
# 3. Optimize visualizations
```

### Issue: Streamlit Cloud deployment failed

**Solution:**
1. Check requirements.txt untuk versi yang kompatibel
2. Pastikan Python version 3.8+ di Streamlit settings
3. Check logs di Streamlit Cloud dashboard
4. Pastikan semua file ada di repository

## 📊 Testing Dashboard Features

Setelah dashboard running, test semua features:

1. **Sidebar Filters**
   - Select different years
   - Select different seasons
   - Change weather conditions
   - Toggle working day options

2. **Tab Overview**
   - Check time series chart
   - Verify box plots
   - Read key insights

3. **Tab Temporal Analysis**
   - View hourly patterns
   - Check day of week analysis
   - Explore heatmap
   - Review monthly trends

4. **Tab Weather Impact**
   - Analyze weather conditions
   - Check temperature scatter plot
   - Review humidity impact
   - Read weather statistics table

5. **Tab User Segmentation**
   - Compare casual vs registered
   - View working day patterns
   - Analyze weekend behavior

6. **Tab Clustering**
   - Adjust number of clusters
   - View PCA visualization
   - Read cluster characteristics
   - Review recommendations

## 🎯 Expected Results

Setelah semua setup:

1. **Notebook Output**
   - All cells executed successfully
   - All visualizations rendered
   - Statistical results displayed
   - Insights clearly stated

2. **Dashboard**
   - Loads in < 5 seconds
   - All tabs functional
   - Filters update visualizations
   - No errors in browser console

3. **GitHub Repository**
   - Clean directory structure
   - All files present
   - README comprehensive
   - Code well-commented

## 🎓 Grading Expectations

**60 Points**: Basic requirements met
- Dataset present
- Notebook runs
- Dashboard functional

**70 Points**: Standard analysis
- Basic statistics (mean, count, etc.)
- Simple visualizations
- Working dashboard

**80 Points**: Advanced analysis
- Clustering implemented
- Time series analysis
- Advanced visualizations
- Interactive dashboard

**90 Points**: Excellent work
- Multiple advanced techniques
- Professional documentation
- Comprehensive insights
- Strategic recommendations
- Clean, well-structured code

## 🆘 Need Help?

1. **Check Documentation**
   - README.md untuk overview
   - DEPLOYMENT_GUIDE.md untuk deployment
   - Notebook comments untuk analisis

2. **Common Resources**
   - [Streamlit Docs](https://docs.streamlit.io/)
   - [Pandas Docs](https://pandas.pydata.org/docs/)
   - [Plotly Docs](https://plotly.com/python/)
   - [Scikit-learn Docs](https://scikit-learn.org/)

3. **Ask for Help**
   - Open GitHub issue
   - Check with classmates
   - Consult with instructor

## 🎉 Success!

Jika semua checklist ✅, Anda siap untuk submit!

Good luck dan semoga berhasil! 🚀

---

**Next Steps:**
1. Run local testing → ✅
2. Push to GitHub → ✅
3. Deploy to Streamlit → ✅
4. Record video → ✅
5. Submit → ✅
6. Celebrate! 🎊
