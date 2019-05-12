[![Build Status](https://travis-ci.org/avh4/elm-json-mapping.svg?branch=master)](https://travis-ci.org/avh4/elm-json-mapping)
[![Latest Elm package version](https://img.shields.io/elm-package/v/avh4/elm-json-mapping.svg?label=elm)][elm-package]


[Elm]: https://elm-lang.org/
[elm-package]: https://package.elm-lang.org/packages/avh4/elm-json-mapping/latest/


## Usage

```elm
import Json.Mapping exposing (object, withString, withInt)

type alias Model =
    { name : String
    , count : Int
    }
    
    
mapping : JsonMapping Model Msg
mapping =
    object Loaded
        |> withString "name" .name
        |> withInt "count" .count
```

