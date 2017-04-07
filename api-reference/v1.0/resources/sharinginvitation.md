# <a name="sharinginvitation-resource-type"></a>Тип ресурса SharingInvitation

Ресурс **SharingInvitation** — это единая структура, объединяющая элементы данных, связанные с приглашениями.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a>Свойства

| Имя свойства  | Тип                          | Описание                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| email          | String                        | Электронный адрес получателя приглашения к совместному использованию. Только для чтения.                                          |
| invitedBy      | [identitySet](identityset.md) | Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения. |
| signInRequired | Логическое                       | Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.                     |

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingInvitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
