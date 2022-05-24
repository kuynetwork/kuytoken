# KUY TOKEN

**Ticker Token**

- Name: Kuy Token
- Symbol: KUY
- Decimal: 18

**Interface**

- IERC20 renamed IKUY20
- IUniswapV2Factory
- IUniswapV2Pair
- IUniswapV2Router01
- IUniswapV2Router02

**included library**

- SafeMath
- Address
- Ownable
- Context

**Set Symbol Name and Decimal Token**

>      string  private _name = "Kuy Token";
>
>      string  private _symbol = "KUY";
>
>      uint8  private _decimals = 18;

**Mint Max Supply**

    _mint(_msgSender(), 100000000 * 10**uint256(_decimals))

> 100 Milion supply 18 Decimal

**Burn Address**

> `address public burnAddress = 0x0000000000000000000000000000000000000000`;

**IUniswapV2Router02**

    IUniswapV2Router02 _uniswapV2Router = IUniswapV2Router02(

    0x10ED43C718714eb63d5aA57B78B54704E256024E

    );

Note

> 0x10ED43C718714eb63d5aA57B78B54704E256024E
> is pancakeswap Router address

** Function For Get Current Burn**

    function  getCurrentBurn() public  view  returns (uint256) {

    return _curentBurn;

    }

**Additional**:

> for detailed documentation on the function please read the comments in the <a href="https://github.com/vexanium/KUY/blob/main/contracts/kuy.sol">Code</a>
