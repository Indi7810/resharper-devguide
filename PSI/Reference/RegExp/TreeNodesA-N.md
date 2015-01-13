# TreeNodes A - N

<!-- Index A - N (auto-generated. Remove this line if manually adding/removing entries) -->

<!-- toc -->
<!-- toc stop -->

## A

### IAlternationGroup

<!-- Begin IAlternationGroup -->

```cs
public interface IAlternationGroup :
  IGroup,
  IQuantifierOwner,
  IRegExpTreeNode,
  ITreeNode
{
  ITokenNode AltLParenth { get; }
  ITokenNode AltRParenth { get; }
  ITokenNode LongPrefix { get; }
  ITokenNode Pipe { get; }
  ITokenNode Prefix { get; }
  ITokenNode QuestionSign { get; }
}
```

<!-- End IAlternationGroup -->

### IAnchor

<!-- Begin IAnchor -->

```cs
public interface IAnchor :
  IUnitRegularExpression,
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End IAnchor -->

## B

### IBorderAnchor

<!-- Begin IBorderAnchor -->

```cs
public interface IBorderAnchor :
  IAnchor,
  IUnitRegularExpression,
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End IBorderAnchor -->

### IBracketCharacter

<!-- Begin IBracketCharacter -->

```cs
public interface IBracketCharacter :
  ICharacter,
  IQuantifierOwner,
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End IBracketCharacter -->

## C

### ICharacter

<!-- Begin ICharacter -->

```cs
public interface ICharacter :
  IQuantifierOwner,
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End ICharacter -->

### IConcatenationRegularExpression

<!-- Begin IConcatenationRegularExpression -->

```cs
public interface IConcatenationRegularExpression :
  IRegExpTreeNode,
  ITreeNode
{
  TreeNodeCollection<IUnitRegularExpression> UnitRegularExpressions { get; }
  TreeNodeEnumerable<IUnitRegularExpression> UnitRegularExpressionsEnumerable { get; }
}
```

<!-- End IConcatenationRegularExpression -->


## E

### IEndAnchor

<!-- Begin IEndAnchor -->

```cs
public interface IEndAnchor :
  IAnchor,
  IUnitRegularExpression,
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End IEndAnchor -->

### IEscapeCharacter

<!-- Begin IEscapeCharacter -->

```cs
public interface IEscapeCharacter :
  ICharacter,
  IQuantifierOwner,
  ISetBodyCharacter,
  ISetBodyItem,
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End IEscapeCharacter -->

## G

### IGroup

<!-- Begin IGroup -->

```cs
public interface IGroup :
  IQuantifierOwner,
  IRegExpTreeNode,
  ITreeNode
{
  ITokenNode LParenth { get; }
  ITokenNode RParenth { get; }
}
```

<!-- End IGroup -->

### IGroupName

<!-- Begin IGroupName -->

```cs
public interface IGroupName :
  IRegExpTreeNode,
  ITreeNode
{
  ITokenNode Dash { get; }
  ITokenNode Gt { get; }
  ITokenNode Lt { get; }
  IName Name { get; }
  IName SecondaryName { get; }

  IName SetName(IName param);
  IName SetSecondaryName(IName param);
}
```

<!-- End IGroupName -->

### IGroupPrefix

<!-- Begin IGroupPrefix -->

```cs
public interface IGroupPrefix :
  IRegExpTreeNode,
  ITreeNode
{
  ITokenNode LongPrefix { get; }
  ITokenNode Lt { get; }
  ITokenNode Prefix { get; }
}
```

<!-- End IGroupPrefix -->


## I

### IInvalidCharacter

<!-- Begin IInvalidCharacter -->

```cs
public interface IInvalidCharacter :
  IErrorElement,
  ICharacter,
  IQuantifierOwner,
  ISetBodyCharacter,
  ISetBodyItem,
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End IInvalidCharacter -->

## N

### IName

<!-- Begin IName -->

```cs
public interface IName :
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End IName -->

### INamedBackreference

<!-- Begin INamedBackreference -->

```cs
public interface INamedBackreference :
  IRegExpTreeNode,
  ITreeNode
{
  ITokenNode Gt { get; }
  ITokenNode Lt { get; }
  IName Name { get; }

  IName SetName(IName param);
}
```

<!-- End INamedBackreference -->

### INamedBlock

<!-- Begin INamedBlock -->

```cs
public interface INamedBlock :
  IRegExpTreeNode,
  ITreeNode
{
  ITokenNode LBrace { get; }
  IName Name { get; }
  ITokenNode RBrace { get; }

  IName SetName(IName param);
}
```

<!-- End INamedBlock -->

### INamedGroup

<!-- Begin INamedGroup -->

```cs
public interface INamedGroup :
  IGroup,
  IQuantifierOwner,
  IRegExpTreeNode,
  ITreeNode
{
  IGroupName GroupName { get; }
  ITokenNode QuestionSign { get; }
  IRegularExpression RegularExpression { get; }

  IGroupName SetGroupName(IGroupName param);
  IRegularExpression SetRegularExpression(IRegularExpression param);
}
```

<!-- End INamedGroup -->

### INestedSet

<!-- Begin INestedSet -->

```cs
public interface INestedSet :
  ISetBodyItem,
  IRegExpTreeNode,
  ITreeNode
{
  ITokenNode Dash { get; }
  ISet InnerSet { get; }

  ISet SetInnerSet(ISet param);
}
```

<!-- End INestedSet -->

### INumber

<!-- Begin INumber -->

```cs
public interface INumber :
  IRegExpTreeNode,
  ITreeNode
{
}
```

<!-- End INumber -->

### INumericQuantifier

<!-- Begin INumericQuantifier -->

```cs
public interface INumericQuantifier :
  IRegExpTreeNode,
  ITreeNode
{
  ITokenNode Comma { get; }
  ITokenNode LBrace { get; }
  INumber Number { get; }
  ITokenNode RBrace { get; }
  INumber SecondaryNumber { get; }

  INumber SetNumber(INumber param);
  INumber SetSecondaryNumber(INumber param);
}
```

<!-- End INumericQuantifier -->
