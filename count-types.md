<!-- ⊕ 𝔹 ∈ → ∀ -->

Leibniz:
 - Identity of indiscernibles
 - Indiscernability of identities
 
 Conc: x=y ⇔ ( ∀P.P(x) <=> P(y) )
 
 - |Bool|     = 2
 - |(A,B)|    = |A| x |B|
 - Either A B = |A| + |B|
 - Maybe A    = |A| + 1
 - A -> B     = |B| ^ |A|
 
 - Isomorphism
   data Iso a b {
    to :: a -> b
    from :: b -> a
    -- fromTo :: (x :: a) -> (from . to) x = x
    -- toFrom :: (x :: b) -> (to . from) x = x
   }
   
   
 - Observational equality  x=y ⇔ ( ∀P.P(x) <=> P(y) )
 - if A anb B are iso. they have the same number of inhabitants
 
 - pairing :: Iso (Either a b -> c) (a -> c, b -> c)
   - to :: (Either a b -> c) -> (a -> c, b -> c)
   - to f = (\a -> f (Left a), \b -> f (Right b))
 
   - from :: (a -> c, b -> c) -> (Either a b -> c)
   - from (ac, bc) =
   
   
 - (∀x.(a → x) → f x ∼= f a)  
  
  1. ∀ a b c. (a -> c) -> b -> a -> c
  2. -- newtype F a b x = b -> a -> x
    3. (a -> x) -> F a b x    
  1. ∀ a b c. b -> (a -> c) -> a -> c