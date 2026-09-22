# wheatcrop-java

Objective:

To create an interface Harvestable containing the harvest() method and implement it in the WheatCrop class.


Java Concepts / Syntax Used:

Interface
Interface implementation
implements keyword
Method implementation / overriding
Object creation

Syntax:

interface InterfaceName {
    void methodName();
}

class ClassName implements InterfaceName {
    @Override
    public void methodName() {
        // implementation
    }
}


Algorithm:

Start.
Create the Harvestable interface.
Declare the harvest() method.
Create the WheatCrop class implementing Harvestable.
Implement the harvest() method.
Create an object of WheatCrop.
Call the harvest() method.
Stop.


Java Code:

interface Harvestable {
    void harvest();
}
class WheatCrop implements Harvestable {
    String cropName;

    WheatCrop(String cropName) {
        this.cropName = cropName;
    }

    @Override
    public void harvest() {
        System.out.println(cropName + " is ready for harvest.");
    }
}

public class HarvestDemo {
    public static void main(String[] args) {
        WheatCrop wheat = new WheatCrop("Wheat");
        wheat.harvest();
    }
}


Output:

Wheat is ready for harvest.