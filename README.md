# tsemodule5
# # User Manual for tsemodule5
# ### Code by @Pythonfinance
# #### t.me/python4finace
# #### www.python4finace.ir

# In[1]:


import tsemodule5 as tm5
import mplfinance


# ## show the list of all iran stock tickers 
# Function stockdetail have some parameters:
# stockdetail(tikcer,type)
# if you set ticker to "list" it show all tickers and names.

# In[2]:


tm5.stockdetail("list")


# ## show full information about a tickers 

# In[3]:


tm5.stockdetail("شبندر")


# ## show english ticker name 

# In[4]:


tm5.stockdetail("شبندر",type="namadf")


# ## show english ticker name by full farsi name 

# In[5]:


tm5.stockdetail("پالايش نفت بندرعباس",type="name")


# ## show full farsi name by english ticker name

# In[6]:


tm5.stockdetail("PNBA1",type="enamad")


# ## show all ticker names 
# use it for analysis some functions on the market stocks
# 

# In[7]:


tm5.stocklist()


# ## show the stock information for 100 last days

# In[8]:


tm5.stock("شبندر")


# show the stock information for custom last days

# In[9]:


tm5.stock("شبندر",value=10)


# ## Download information from the server or read from local

# In[10]:


tm5.stock("شبندر",newfile=True)


# ## Get stock information like yahoo-finance
# use it for polt in mplfinance or other standard modules

# In[11]:


tm5.stock("شبندر",value=10,standard=True)


# # Get stock information by english ticker name
# use it if you know english ticker name

# In[12]:


tm5.stock("PNBA1",value=10,standard=True,namadf=False)


# ## Example:
#     plot the OHLC for tikcer شبندر for 50 last days

# In[13]:


mplfinance.plot(tm5.stock("شبندر",value=50,standard=True))

