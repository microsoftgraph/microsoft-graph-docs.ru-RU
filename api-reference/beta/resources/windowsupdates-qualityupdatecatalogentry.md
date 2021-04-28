---
title: тип ресурса qualityUpdateCatalogEntry
description: Метаданные для обновления Windows 10 качества, которое можно утвердить для развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f455919bfc3d5f0e6c4e2aa5ef6a6b630b66bc52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068082"
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
|id|String|Уникальный идентификатор для записи каталога. Только для чтения. Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).|
|isExpeditable|Логический|Указывает, можно ли развертывать контент в качестве ускоренного обновления качества. Только для чтения.|
|qualityUpdateClassification|microsoft.graph.windowsUpdates.qualityUpdateClassification|Классификация обновления качества. Поддерживает подмножество значений **для qualityUpdateClassification.** Возможные значения: `all`, `security`, `nonSecurity`. Только для чтения.|
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

