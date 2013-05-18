<?xml version="1.0" encoding ="utf-8"?>
<!ELEMENT car (ad+)>
<!ELEMENT ad (make, model, year, color, engine number_of_doors, transmition_type, accessoies)>
<!ELEMENT make (#PCDATA)>
<!ELEMENT model (#PCDATA)>
<!ELEMENT engine (no_of_cyleder, fuel_system)>
<!ELEMENT no_of_cylender (#PCDATA)>
<!ELEMENT fuel_system (#PCDATA)>

<!ELEMENT no of cylender (#PCDATA)>
<!ELEMENT fuel system (#PCDATA)>
<!ELEMENT year (#PCDATA)>
<!ELEMENT color (#PCDATA)>
<!ELEMENT transmition_type (#PCDATA)>
<!ATTLIST car 
              accessories radio CDATA #REQUIRED
              accessories air_conditionig CDATA #REQUIRED
        accessories power_windows CDATA #REQUIRED
              accessories power_steering CDATA #REQUIRED
              accessories power breaks CDATA #REQUIRED
>
  
 
<!ENTITY m " Mercidies ">
<!ENTITY s " Swift ">


THE XML FILE FOR ABOVE DTD FILE IS AS FALLOWS

<?xml version="1.0" encoding ="utf-8"?>
<!DOCTYPE cars SYSTEM "cars.dtd">
<cars>
<ad>
        <make> &m; </make>
  <year> 1990 </year>
	<model> 2000 </model>
	<color> red </color>
	<no_of_doors> 4 </no_of_doors>
	<transmition_type> fuel </transmition_type>
	<engine>
		<no_of_cylender> 4 </no_of_cylender>
		<fuel_system> petrol </fuel_system>
	</engine>
	<accessories>
		<radio> yes </radio>
		<airconditioning> yes </airconditioning>
		<power_steering> yes </power_steering>
		<power_windows> yes </power_windows>
		<power_break> yes </power_break>
	</accessories>
</ad>

<ad>
	<year> 1991 </year>
	<make> &s; </make>
	<model> 2002 </model>
 	<color> white </color>
	<no_of_doors> 2 </no_of_doors>
	<transmition_type> fuel </transmition_type>
	<engine>
		<no_of_cylender> 6 </no_of_cylender>
		<fuel_system> disel </fuel_system>
	</engine>
	<accessories>
		<radio> yes </radio>
		<airconditioning> yes </airconditioning>
		<power_steering> yes </power_steering>
		<power_windows> yes </power_windows>
		<power_break> yes </power_break>
	</accessories>
</ad>
	</cars>








