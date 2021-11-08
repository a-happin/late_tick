corelib.post_tick.datapack
==

## Features

- `#tick`のあとに任意の`function`を実行する
- ※`schedule tick`で実行されます
  - ので、ここで`/schedule`をすると1tick遅れます

## Usage

1. `function your_namespace:post_tick`などにmcfunctionを定義
1. `tag/function #minecraft:post_tick/N`を作成、上で作ったmcfunctionを入れる。

- `N`は`00`~`99`
- データパックの優先度が高いほど`N`を低くすると良い。
- 前提データパックは0に近い値にする。
- mainは50くらい?それとも99?→99で良いと思うけど99より後ろがないので90が安牌な気がする。
- 数字がかぶっても順番がちょっとおかしくなるだけで特に問題はない。依存関係があるものは数字をちゃんとする。
- Nが高いほど先に実行される(`core:tick`→`main:tick`→`main:post_tick`→`core:post_tick`)
  - 先にtickするdatapackのpost_tickは後に実行させたい場合が多いはずなので

## Requirement

## Installation

## License
Creative Commons Zero v1.0 Universal
