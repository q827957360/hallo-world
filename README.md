# hallo-world
public void remove(Map<String,String> map){
  Set<String> values = new HashSet<>();
  Iterator<Entry<String,String>> it = map.entrySet().iterator();
  while(it.hasnext()){
    Entry<String,String> entry = it.next();
    if(values.contains(entry.getValue())){
      it.remove();
    }else{
      values.add(entry.getValue());
    }
  }
}
