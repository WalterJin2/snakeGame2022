算法: 
蛇数据结构 snakeDots=[[尾left, 尾Top],...,[头left, 头Top]]
蛇大小=
    position: absolute;
    width: 2%;
    height: 2%;
蛇位置=
      {props.snakeDots.map((dot, i) => {
        const style = {
          left: `${dot[0]}%`,
          top: `${dot[1]}%`
        }
        return (
          <div className="snake-dot" key={i} style={style}></div>
        )
      })}
