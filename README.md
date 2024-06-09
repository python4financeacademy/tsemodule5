# tsemodel7

![image](https://github.com/Peyman2012/tsemodule7/assets/88220773/cf3d963a-219b-46bc-b096-df52af9877c1)


A library for managing stock and index data from TSETMC.

### Project folder structure:

    tsemodel7/
    │
    │
    ├── tsemodule7.py
    └── README.md

### Example:

    from tsemodel7 import StockManager, IndexManager

    stock_manager = StockManager()
    index_manager = IndexManager()

    # Example calls
    print(stock_manager.stocklist())
    print(stock_manager.stock("آپ", value=10, standard=True))
    print(index_manager.index(value=10))


### Output FROM StockManager Class:
![image](https://github.com/Peyman2012/tsemodule7/assets/88220773/924892d8-1eb5-477a-a0bc-9ef9bcf8de62)

### Output FROM IndexManager Class:
![image](https://github.com/Peyman2012/tsemodule7/assets/88220773/389a83bd-0ff5-463a-b082-b3dba183b430)







