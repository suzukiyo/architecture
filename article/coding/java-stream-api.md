## java stream api, 順序保証のgroupingby

```
✕　これではMapの順序が保証されなかった
Map<Date, List<Message>> messagesByDate = messages.messages().list().stream()
.collect(Collectors.groupingBy(Message::sendDate));

○　LinkedHashMapを明示してあげることで解決した
Map<Date, List<Message>> messagesByDate = messages.messages().list().stream()
.collect(Collectors.groupingBy(Message::sendDate, LinkedHashMap::new, toList()));
```
