# <a name="publicationfacet-resource-type"></a>Тип ресурса publicationFacet

Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a>Свойства

|   Свойство    |  Тип  | Описание |
| :------------ | :----- | :---------- |
| **level**     | Cтрока | Состояние публикации для данного документа. Возможные значения: `published` или `checkout`. Только для чтения.  |
| **versionId** | Cтрока | Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта. Только для чтения.  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
