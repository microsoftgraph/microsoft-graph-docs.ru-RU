# <a name="helpers-examples-that-arent-included-in-the-docs"></a>Вспомогательный код (примеры, не включенные в документы)

Ниже представлены фрагменты, которые пришлось добавить в документы, чтобы средство Markdown-Scanner могло правильно обработать документы по Graph.


## <a name="define-the-me-as-singleton"></a>Определение /me как одноэлементного класса

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a>Определение drives как набора EntitySet, поддерживающего запросы
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a>Определение users как EntitySet, поддерживающего запросы

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK

{
}
```
