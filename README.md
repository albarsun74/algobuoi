# algobuoi

import datetime as dt
import matplotlib.pyplot as plt
from matplotlib import style
import pandas as pd
import pandas_datareader.data as web

style.use('ggplot')

start = dt.datetime(2021, 5, 1)
end = dt.datetime(2021, 5, 22)

df = web.DataReader("NFLX", "yahoo", start, end)
print(df.head())
