# GPU Data Science

> Okay, so they are giving us cloud IP addresses to log into, so I may not have much to share here, except my notes.

## Notes

* Fun! They provide a cloud instance for everyone in the room, so we can play with a machine with sufficient GPU power.
* The old solution: Hadoop, but that had too much IO. So people moved to Spark.
* RAPIDS is Nvidia's GPU architecture
* RAPIDS uses Apache Arrow (which tries to standardize the storage of columnar data in memory)
* cuDF has nearly identical syntax to Pandas DataFrames
   * The API for cuDF is super handy, I'll give them that.
   * I guess that means you can also use cuDF as a drop-in replacement in your code base... I see.
* String Example: big string replace operations on pd.DataFrame
   * 50x speed-up using cuDF and fixed-length NumPy strings
   * TODO: Whoops. At work, are we not converting our strings in pd.DataFrames to NumPy string arrays?
* [RAPIDS docs](https://docs.rapids.ai/)
* [Play around with RAPIDS](https://rapids.ai/start.html)
* [cuDF GitHub](https://github.com/rapidsai/cudf)
* [cupy](https://cupy.chainer.org/) is a replacement for NumPy, but in the GPU

