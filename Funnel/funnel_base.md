
## pyecharts 代码 / 效果

```python
from pyecharts import options as opts
from pyecharts.charts import Funnel
from pyecharts.faker import Faker

c = (
    Funnel()
    .add("商品", [list(z) for z in zip(Faker.choose(), Faker.values())])
    .set_global_opts(title_opts=opts.TitleOpts(title="Funnel-基本示例"))
    .render("funnel_base.html")
)

```

<iframe width="100%" height="800px" src="Funnel/funnel_base.html"></iframe>