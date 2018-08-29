# <a name="mediacontentratingfrance-resource-type"></a>Тип ресурса mediaContentRatingFrance

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|оценка фильма|[оценка Тип фильма во Франции](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|Оценка выбранных для Франции фильмов. Допустимые значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`,`agesAbove18`.|
|тв оценка|[оценка типа телевидения во Франции](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|ТВ-оценка, выбранная для Франции. Допустимые значения: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`,`agesAbove18`.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



