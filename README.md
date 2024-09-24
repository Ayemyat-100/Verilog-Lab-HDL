//Exercise Q-3

module testbench_oneBitFA1;
    reg a_i, b_i, ci_i;
    wire sum_o, co_o;
    
    // Instantiate the oneBitFA1 module
    oneBitFA1 uut (
        .a_i(a_i),
        .b_i(b_i),
        .ci_i(ci_i),
        .sum_o(sum_o),
        .co_o(co_o)
    );

    initial begin
        // Apply input combinations
        $monitor("a_i = %b, b_i = %b, ci_i = %b -> sum_o = %b, co_o = %b", a_i, b_i, ci_i, sum_o, co_o);
        a_i = 0; b_i = 0; ci_i = 0; #10;
        a_i = 0; b_i = 0; ci_i = 1; #10;
        a_i = 0; b_i = 1; ci_i = 0; #10;
        a_i = 0; b_i = 1; ci_i = 1; #10;
        a_i = 1; b_i = 0; ci_i = 0; #10;
        a_i = 1; b_i = 0; ci_i = 1; #10;
        a_i = 1; b_i = 1; ci_i = 0; #10;
        a_i = 1; b_i = 1; ci_i = 1; #10;
        $finish;
    end
endmodule

------------------xxxx---------------------xxxx------------------xxxx------------------xxxx--------------------xxxx

module testbench_oneBitFA2;
    reg a_i, b_i, ci_i;
    wire sum_o, co_o;
    
    // Instantiate the oneBitFA2 module
    oneBitFA2 uut (
        .a_i(a_i),
        .b_i(b_i),
        .ci_i(ci_i),
        .sum_o(sum_o),
        .co_o(co_o)
    );

    initial begin

        // Apply input combinations
        $monitor("a_i = %b, b_i = %b, ci_i = %b -> sum_o = %b, co_o = %b", a_i, b_i, ci_i, sum_o, co_o);

        a_i = 0; b_i = 0; ci_i = 0; #10;
        a_i = 0; b_i = 0; ci_i = 1; #10;
        a_i = 0; b_i = 1; ci_i = 0; #10;
        a_i = 0; b_i = 1; ci_i = 1; #10;
        a_i = 1; b_i = 0; ci_i = 0; #10;
        a_i = 1; b_i = 0; ci_i = 1; #10;
        a_i = 1; b_i = 1; ci_i = 0; #10;
        a_i = 1; b_i = 1; ci_i = 1; #10;
        $finish;

    end
endmodule


                                

