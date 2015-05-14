/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package asd4;

    class Asd4 {
    private String[] data;
    private int top;
    
    Asd4 (int size) {
        data = new String[size];
        top  = -1;
    }
    
    public void push (String inData) {
        top++;
        data[top] = inData;
    }
    
    public String pop(){
        return data[top--];
    }
}
    class Coba {
    public static void main(String[] args) {
        Asd4 summon = new Asd4(3);
        summon.push("Anjing");
        summon.push("Ngentod");
        summon.push("Jembut");
        
        System.out.println(summon.pop());
        System.out.println(summon.pop());
        System.out.println(summon.pop());
    }
    }
