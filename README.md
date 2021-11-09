# travel_ui

## flutter version 2.5.1  and  null-safety-package
```
  cupertino_icons: ^1.0.2
  font_awesome_flutter: ^9.2.0
```

## accentColor 过期 colorScheme.secondary代替

```
        color: Theme.of(context).accentColor
        color: Theme.of(context).colorScheme.secondary,
```
        
## list<IconData> map to list<Icon>
```
Row(
              mainAxisAlignment: MainAxisAlignment.spaceAround,
              children:
                  _icons.asMap().entries.map((e) => _buildIcon(e.key)).toList(),
            ),

```

## image radius

```
                            ClipRRect(
                              borderRadius: BorderRadius.circular(20),
                              child: Image(
                                image: AssetImage(destination.imageUrl ?? ''),
                                height: 180,
                                width: 180,
                                fit: BoxFit.cover,
                              ),
                            ),


```

