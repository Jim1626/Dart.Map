import 'dart:async';

void main() {
  Map<String, String> parson = {
    'Name': 'Jim',
    'Age': '23',
    'Addr': 'Joypurhat',
    'Expr': '0.1 year',
  };
  print(parson);
  print('Name:${parson['Name']}');
  print('Age: ${parson['Age']}');
  print('Expe: ${parson['Expr']}');
  parson['Expr'] = '2years';
  print('Expr: ${parson['Expr']}');
  parson.addAll({
    'University': 'SUB',
    'Program': 'CSE',
    'ID': 'UG02-63-23-007',
  });
  print(parson);
  print(parson.containsKey('phone number'));
  print(parson.containsKey('ID'));
  print(parson.containsValue('UG02-63-23-007'));
  print(parson.containsKey('Jemi'));
  Map<String, String> Aditionalinfo = {
    'CGPA': '2.88',
    'Phone number': '01403648451',
    'Bus rut': 'Jigatola',
  };
  print(Aditionalinfo);
  print(parson);
  print(
    'parson: $parson'
    'Aditionalinfo:$Aditionalinfo',
  );
  print(parson.length);
  print(Aditionalinfo.length);
  var keylist = parson.keys.toList();
  print(parson.keys);
  print(Aditionalinfo.keys);
  print(keylist);
  print(parson.runtimeType);
  print(Aditionalinfo.runtimeType);
  print(keylist.runtimeType);
  parson.clear();
  print(parson);
  Aditionalinfo.clear();
  print(Aditionalinfo);
}
