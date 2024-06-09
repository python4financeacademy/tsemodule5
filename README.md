### Project folder structure

    tsemodel7/
    │
    ├── tsemodel7/
    │   ├── __init__.py
    │   ├── stock_manager.py
    │   └── index_manager.py
    │
    ├── setup.py
    └── README.md

# tsemodel7

A library for managing stock and index data from TSETMC.

## Installation

You can install the library using pip:

```bash

    pip install tsemodel7

    from tsemodel7 import StockManager, IndexManager

    stock_manager = StockManager()
    index_manager = IndexManager()

    # Example calls
    print(stock_manager.stocklist())
    print(stock_manager.stockdetail("آبادا", type="full"))
    print(stock_manager.stock("آپ", value=10))
    print(index_manager.index(value=10))





