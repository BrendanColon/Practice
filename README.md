# Practice

Data in a comma separated file servo.data, looks as follows

E,E,5,4, 0.28125095

B,D,6,5, 0.5062525

D,D,4,3, 0.35625148

etc.

When this is read into a variable and given column names I can't slice by column name without getting an error
```{r}
servo = pd.read_csv('servo.data', names=['motor', 'screw', 'pgain', 'vgain', 'class'])
servo.loc['vgain']
```

KeyError: 'the label [vgain] is not in the [index]'

How can I properly index the column names?

