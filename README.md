# Commodity Futures Swaption Model


A commodity futures swaption (CFSn) is a linear portfolio of options on FCCF. Hence it suffices to consider one option on an FCCF. Suppose that the underlying FCCF has a maturity of settlement Tfccf , a commodity principal P, average time points t1 < ¢ ¢ ¢ < tn <Tfccf , average weights f!1; ¢ ¢ ¢ ; !ng, and an index ¯. Let T be a maturity of the option onthe FCCF where T < t1 and KC2comm be a strike of the option. Now let VC1(t; ¯) be the value at time t of the option on the ¯-FCCF. From the FCCF pricing formula (6), the payoff of the option at the maturity T becomes

 

It is clearly to see that

 

By the no-arbitragy pricing theory, we have

 

which is called the put-call parity for options on FCCF. If we could find exact solution for either VC1(t; 1) or VC1(t;¡1), then we may get the exact solution for the other. However, in real life, we can get precise solution for neither of them. Only approximate solutions are available. In some cases, having an approximate solution for ¯ = 1, it is not a good idea to get the one for ¯ = ¡1 by using the put-call parity. Thus we have to consider both cases of ¯ = 1 and ¯ = ¡1 (see https://finpricing.com/lib/FiBondCoupon.html)

Besides the assumption proposed in the previous sections, it is also assumed that the commodity price and the currency exchange rate follow geometric Brownian motions with deterministic volatilities. The correlative coefficient between the commodity futures and the exchange rate is assumed to be constant. Applying Vorst’s approximation, we have

 

where © is the standard normal cumulative distribution function, K¤, ¹, v, and details of derivations are given

Let FC(t; I) be the futures price corresponding to some futures contract with index I in the C-currency. The first result states that the futures price process FC(t; I) is a martingale in the C-risk-neutral world, i.e.,
for s < t,

 

Let t < t0, XC be a random payoff in C-currency which is measurable at time t0 and SC0C is currency exchange rate between currencies C and C0. Then we have the second result that

 

where fC0C is the forward exchange rate between currencies C and C0. This also tells us that if X is a martingale in the C-risk-neutral world up to a time T0, then it may not be a martingale in the C0-risk-neutral world. However, fC0C (¢; t0) ¢ X is a martingale in the C0-risk-neutral world for any given t0 · T0.

Let us consider a European derivative with a matured payoff given by VC1(T) in the C1-currency world, where T is the maturity. then we have, for any time t < T,

 

Consider the above derivative in the C2-currency world. i.e., we have the derivative with the matured payoff given by VC2(T) = SC2C1 (T) ¢ VC1(T). The third result tells us that, for any time t < T,

 


