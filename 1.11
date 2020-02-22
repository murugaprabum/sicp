# Exercise 1.11 in SICP
defmodule Exercise1point11 do

  def recursive(n) when n < 3 do
    n
  end

  def recursive(n) do
    recursive(n-1) + (2 * recursive(n-2)) + (3 * recursive(n-3))
  end

  def iterative(n) do
    case n do
    0 -> 0
    1 -> 1
    2 -> 2
    _ -> iteativeinternal(0, 1, 2, n)
    end
    
  end

def iteativeinternal(a, b, c, count) do
  case count do
    count when count <= 2 -> c
    _ -> iteativeinternal(b, c, c + (2 * b) + (3 * a), count - 1)
  end
end

end

IO.puts(Exercise1point11.recursive(10))
IO.puts(Exercise1point11.recursive(1))

IO.puts(Exercise1point11.iterative(10))
IO.puts(Exercise1point11.iterative(1))
