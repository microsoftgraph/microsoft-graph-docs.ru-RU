---
title: тип ресурса qualityUpdateCatalogEntry
description: Метаданные для обновления Windows 10 качества, которое можно утвердить для развертывания.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 23301d5de5d089ed47dc884ad62a88b0660cd0ec
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891181"
---
# <a name="qualityupdatecatalogentry-resource-type"></a>тип ресурса qualityUpdateCatalogEntry

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Метаданные для обновления Windows 10 качества, которое можно утвердить для развертывания.

Windows 10 обновления качества выпускаются один или несколько раз в месяц. Эти обновления содержат исправления безопасности и качества и обычно выпускаются во второй вторник каждого месяца, хотя они могут быть выпущены в любое время. Эти обновления являются накопительными, поэтому более поздние версии всегда содержат все предыдущие исправления. Корпорация Майкрософт настоятельно рекомендует сохранять устройства текущими, устанавливая последние обновления качества, как только они будут доступны. 

Наследует от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|Дата, в которую контент больше не доступен для развертывания с помощью службы. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|displayName|String|Отображение имени контента. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|id|Строка|Уникальный идентификатор для записи каталога. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|isExpeditable|Логическое|Указывает, можно ли развертывать контент в качестве ускоренного обновления качества. Только для чтения.|
|qualityUpdateClassification|microsoft.graph.windowsUpdates.qualityUpdateClassification|Классификация обновления качества. Возможные значения: `all`, `security`, `nonSecurity`, `unknownFutureValue`. Только для чтения.|
|releaseDateTime|DateTimeOffset|Дата выпуска контента. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "isExpeditable": "Boolean",
  "qualityUpdateClassification": "String"
}
```

