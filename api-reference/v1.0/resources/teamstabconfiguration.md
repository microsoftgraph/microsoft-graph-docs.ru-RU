# <a name="teamstabconfiguration-resource-type-open-type"></a>teamsTabConfiguration ресурсов (тип Open)



Параметры, определяющие содержимое [вкладки](teamstab.md). Если вкладки интерактивно настроено, эти сведения задается приложение поставщика вкладки.
В дополнение к указанные ниже свойства некоторые приложения поставщика вкладки укажите дополнительные настраиваемые свойства.

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|-|-|-|
|  entityId   |   string |  Идентификатор для сущности, размещенного поставщиком вкладки.     |
|  contentUrl |   string |  URL-адрес, используемый для отображения содержимого вкладки в группах. Обязательно указывать.    |
|  removeUrl  |   string |  URL-адрес, вызванный клиентом команды при удалении вкладки с помощью команды клиента.     |
|  websiteUrl |   string |  URL-адрес для отображения содержимого вкладки вне группы.     |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
