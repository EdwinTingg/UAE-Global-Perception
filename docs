
from pyecharts import options as opts
from pyecharts.charts import WordCloud

data = [
    ("Oil", 100),
    ("Human Rights", 100),
    ("Migrant Workers", 95),
    ("Financial Hub", 95),
    ("Money Laundering", 85),
    ("Geopolitics", 85),
    ("FDI", 85),
    ("Energy Transition", 85),
    ("Climate Change", 80),
    ("Labor Exploitation", 90),
    ("Middle East", 90),
    ("Freedom of Expression", 90),
    ("Kafala System", 85),
    ("Authoritarianism", 75),
    ("OPEC", 75),
    ("Fossil Fuels", 85),
    ("Dubai", 90),
    ("Capital Flows", 80),
    ("Sudan Conflict", 80),
    ("Censorship", 80),
    ("AML", 80),
    ("Islam", 75),
    ("Offshore Finance", 75),
    ("Arms Trade", 75),
    ("COP28", 75),
    ("Renewable Energy", 75),
    ("Human Trafficking", 75),
    ("Surveillance", 75),
    ("FDI", 85),
    ("Real Estate", 70),
    ("Tax Avoidance", 75),
    ("International Trade", 65),
    ("Sovereign Wealth Fund", 65),
    ("Press Freedom", 80),
    ("Democracy", 60),
    ("Religious Tolerance", 65),
    ("Saudi Arabia", 70),
    ("Iran", 65),
    ("China", 65),
    ("United States", 65),
    ("Green Finance", 60),
    ("Carbon Emissions", 80),
    ("Tourism", 75),
    ("Expatriates", 70),
    ("Sharia Law", 60),
    ("Water Scarcity", 55),
    ("Diplomatic Mediation", 55),
    ("Cryptocurrency", 55),
    ("Global City", 60),
]

# 合并重复词汇
from collections import defaultdict
merged = defaultdict(int)
for word, weight in data:
    merged[word] += weight

data = list(merged.items())

wc = (
    WordCloud()
    .add(
        series_name="UAE Global Issues",
        data_pair=data,
        word_size_range=[15, 90],
        shape="circle",
    )
    .set_global_opts(
        title_opts=opts.TitleOpts(
            title="United Arab Emirates",
            subtitle="Global Perceptions and International Issues"
        ),
        tooltip_opts=opts.TooltipOpts(is_show=True),
    )
)

wc.render("docs/index.html") 
