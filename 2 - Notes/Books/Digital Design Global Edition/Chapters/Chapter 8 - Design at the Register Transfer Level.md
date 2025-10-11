# [[Digital Design Global Edition.pdf#page=447&offset=,,|1 - Introduction]]
# [[Digital Design Global Edition.pdf#page=447&offset=,,|2 - Register Transfer Level (RTL) Notation]]
# [[Digital Design Global Edition.pdf#page=449&offset=,,|3 - RTL Descriptions]]
> [!PDF|question] [[Digital Design Global Edition.pdf#page=450&selection=49,0,52,3&color=question|Digital Design Global Edition, p.449]]
> > The following examples show the various ways to specify register transfer operation in Verilog:
> > $$
> > \begin{array}{l l @{\quad} l}
> > 	(a) & \bf{assign} \text{ S = A + B;} & \text{// Continuous assignment for addition operation} \\
> > 	(b) & \bf{always @} \text{ (A, B)} & \text{Level-sensitive cyclic behavior}\\
> > 		& \text{S = A + B;} & \text{Combinational logic for addition operation}\\
> > 	(c) & \bf(always@) \text{ (}\bf{negedge}\text{ clock)} & \text{// Edge-sensitive cyclic behavior}\\
> > \end{array}
> > $$
> 
> So, what exactly is the difference between (a) and (b)? And why would anyone ever use (c)?
> ___
> Well, it is explained just below. An `assign` statement updates when any one of the right-hand side signals change. In other words, the sensitivity list is the right hand side. In (b) the sensitivity list is entered by hand.
> And the other questions is answered here
> > ([[Digital Design Global Edition.pdf#page=451&selection=120,53,125,20|Digital Design Global Edition, p.450]])
> In general, the blocking assignment operator (=) is used in a procedural assignment statement only when it is necessary to specify a sequential ordering of multiple assignment statements, as in a testbench or in combinational logic.

Yeah, I'm not taking note of these. Maybe on a re-read, but unlikely.

# [[Digital Design Global Edition.pdf#page=467&offset=,,|4 - Algorithmic State Machines (ASMs)]]

> [!PDF|important] [[Digital Design Global Edition.pdf#page=471&selection=163,0,164,79&color=important|Digital Design Global Edition, p.470]]
> > Each block in the ASM chart describes the state of the system during one clock-pulse interval (i.e., the interval between two successive active edges of the clock).

