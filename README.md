# tsemodel7

![image](https://github.com/Peyman2012/tsemodule7/assets/88220773/cf3d963a-219b-46bc-b096-df52af9877c1)


A library for managing stock and index data from TSETMC.

### Project folder structure:

    tsemodel7/
    │
    │                   
    ├── tsemodule7.py                     
    |                   
    └── README.md

### Example:

    from tsemodel7 import StockManager, IndexManager

    stock_manager = StockManager()
    index_manager = IndexManager()

    # Example calls
    print(stock_manager.stocklist())
    print(stock_manager.stock("آپ", value=10, standard=True))
    print(index_manager.index(value=10))

### StockManager Class

The StockManager class allows you to easily manage, download, process, and extract information about various stocks. This class can be easily used in different projects and more functionality can be added to it by adding new features and methods.

### Output FROM StockManager Class:
![image](https://github.com/Peyman2012/tsemodule7/assets/88220773/924892d8-1eb5-477a-a0bc-9ef9bcf8de62)

### IndexManager Class

The IndexManager class allows you to easily manage data related to various stock market indices, download them, process them and extract the information you want. This class can be easily used in different projects and more functionality can be added by adding new features and methods.

### Output FROM IndexManager Class:
![image](https://github.com/Peyman2012/tsemodule7/assets/88220773/389a83bd-0ff5-463a-b082-b3dba183b430)

 ## HighPriceManager Class
This class uses an online source to download stock data and then processes and analyzes the data to find the stock's highest closing price.

Using newfile and standard parameters allows you to have more control over the process of downloading and processing data.
The get_highest_close_price_today method examines only the data from the previous day and displays them in sorted order.
### Example:

    high_price_manager = HighPriceManager()

    # Example calls
    highest_close_prices_df = high_price_manager.get_highest_close_price_today(standard=True)
    print(highest_close_prices_df)

### Output FROM HighPriceManager Class:
![image](https://github.com/Peyman2012/tsemodule7/assets/88220773/3472a97e-5bf6-4259-aa0b-b9fda93eb11f)










