### Member Function

```luceescript+trycf
{"RESULT":{"COLUMNS":["ROLEID","ROLE"],"DATA":[[33,"Expert"],[41,"Field User"],[49,"Help Desk Administrator"],[60,"InTouch Administrator"],[80,"InTouch Engineer"],[120,"Publisher"],[101,"Segment Administrator"],[116,"Taxonomy Administrator"]]}};

// Show all animals
Dump(
	label: "COLUMNS",
	var: ROLE
);

// Find animal containing value of 'medium'
findMediumAnimal = animals.findValue("Expert");

// Show results in findMediumAnimal
Dump(
	label: "Results of animals.findValue(""medium"")",
	var: findMediumAnimal
);
```

### Non-Member Function

```luceescript+trycf
animals = {
	cow: {
		noise: "moo",
		size: "large"
	},
	pig: {
		noise: "oink",
		size: "medium"
	},
	cat: {
		noise: "meow",
		size: "small"
	}
};

// Show all animals
Dump(
	label: "All animals",
	var: animals
);

// Find animal containing value of 'medium'
findMediumAnimal = StructFindValue(animals, "medium");

// Show results in findMediumAnimal
Dump(
	label: "Results of StructFindValue(animals, ""medium"")",
	var: findMediumAnimal
);
```
