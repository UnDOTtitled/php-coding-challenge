# Untitled PHP Code Challenge

Here at [Untitled](http://un.titled.co.uk) we are geeks through and through. As such, we would like you to spend 30 minutes pondering this little challenge. We'd like you to use the latest greatest PHP techniques you know.

For this exercise we would like you to concentrate on the weapons system for a first person shooter we are creating.

Each weapon will have a name, effective range, accuracy rating, sound rating, and damage level. Weapons can also have attachments applied to them. Each attachment will affect the attributes of the weapon. For example a pistol with a silencer attachment will have its sound rating reduced. Below is a list of weapons along with their associated attachments and attribute changes.

---------------------------------------

## Pistol

* Effective Range: 50
* Accuracy Rating: 40
* Sound Rating: 45
* Damage Level: 40

Attachments

| Name       | Effective Range | Accuracy Rating | Sound Rating | Damage Level |
|------------|-----------------|-----------------|--------------|--------------|
| Silencer   | 0               | 0               | -10          | 0            |
| Sight      | 10              | 10              | 0            | 0            |
| Dual Wield | 0               | -5              | 10           | 15           |


## Shotgun

* Effective Range: 20
* Accuracy Rating: 40
* Sound Rating: 70
* Damage Level: 75

Attachments

| Name          | Effective Range | Accuracy Rating | Sound Rating | Damage Level |
|---------------|-----------------|-----------------|--------------|--------------|
| Sight         | 15              | 5               | 0            | 0            |
| Double Barrel | 0               | -5              | 10           | 15           |
| Long Barrel   | 15              | 5               | 0            | 0            |


## Sniper Rifle

* Effective Range: 85
* Accuracy Rating: 85
* Sound Rating: 60
* Damage Level: 60

Attachments

| Name          | Effective Range | Accuracy Rating | Sound Rating | Damage Level |
|---------------|-----------------|-----------------|--------------|--------------|
| Suppressor    | 0               | -5              | -10          | 0            |
| FMJ Bullets   | -5              | -5              | 0            | 15           |
| Stock         | 0               | 10              | 0            | 0            |

---------------------------------------

We would like you to code these weapons up and then output their values with help from the excellent [TWIG](http://twig.sensiolabs.org/) teplating engine. Simply instantiate the weapons etc in an index file, then pass them through to a twig template for rendering. We would expect that once a weapon is created with its attachments that we can call methods such as `$weapon->getName()`, which will return the original weapon name as well as the attachments applied to it as part of its name. We would also expect to be able to call `$weapon->getEffectiveRange()` to fetch its range with adjustments already applied for the attachments. If you'd like to, you can also provide a nice method to output allof the values.

## Example Output

As an example this is what a shotgun with a sight and long barrel attachment will output:

Name: Shotgun with sight and long barrel  
Effective Range: 50  
Accuracy Rating: 50  
Sound Rating: 70  
Damage Level: 75  

And here is the output of a sniper rifle with a suppresor, FMJ bullets and stock attachments:

Name: Sniper Rifle with suppressor, FMJ bullets and stock  
Effective Range: 80  
Accuracy Rating: 85  
Sound Rating: 50  
Damage Level: 75  
