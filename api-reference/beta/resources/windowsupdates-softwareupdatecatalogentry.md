---
title: тип ресурса softwareUpdateCatalogEntry
description: Метаданные для обновления программного обеспечения, которое можно утвердить для развертывания.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 7103fbb2f6ed62cec5a5e530a10e190ea46067e0
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862778"
---
# <a name="softwareupdatecatalogentry-resource-type"></a>тип ресурса softwareUpdateCatalogEntry

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Метаданные для обновления программного обеспечения, которое можно утвердить для развертывания.

Наследует [из catalogEntry](../resources/windowsupdates-catalogentry.md). Базовый тип [для featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) и [qualityUpdateCatalogEntry.](../resources/windowsupdates-qualityupdatecatalogentry.md)

Это абстрактный тип.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|Дата, в которую контент больше не доступен для развертывания с помощью службы. Только для чтения. Унаследованный от [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|displayName|String|Отображение имени контента. Только для чтения. Унаследованный от [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|id|String|Уникальный идентификатор для записи каталога. Только для чтения. Унаследованный от [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|releaseDateTime|DateTimeOffset|Дата выпуска контента. Только для чтения. Унаследованный от [catalogEntry](../resources/windowsupdates-catalogentry.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

