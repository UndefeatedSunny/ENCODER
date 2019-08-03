VERILOG CODE FOR ENCODER :-

module encoder_verilog (d, a, b, c);

input [0:7] d;

output a;

output b;

output c;

or(a,d[4],d[5],d[6],d[7]);

or(b,d[3],d[2],d[6],d[7]);

or(c,d[1],d[3],d[5],d[7]);

endmodule



TESTBENCH FOR ENCODER :-

module encoder_testbench;

reg [0:7] d;

wire a;

wire b;

wire c;

encoder_verilog uut (.d(d), .a(a), .b(b),.c(c) );

initial begin

    d=8'b10000000;

#10 d=8'b01000000;

#10 d=8'b00100000;

#10 d=8'b00010000;

#10 d=8'b00001000;

#10 d=8'b00000100;

#10 d=8'b00000010;

#10 d=8'b00000001;

#10$stop;

end

endmodule
