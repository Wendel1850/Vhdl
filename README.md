# Vhdl
library IEEE;
use IEEE.STD_LOGIC;
use IEEE.NUMERIC_STD.ALL;

entity contador_4bits is
    Port ( clk : in STD_LOGIC;
           count : out STD_LOGIC_VECTOR (3 downto 0));
end contador_4bits;

architecture Behavioral of contador_4bits is
    signal count_reg : unsigned (3 downto 0) := (others => '0');
    
