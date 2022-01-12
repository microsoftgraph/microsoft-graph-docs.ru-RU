---
title: тип ресурса catalogEntry
description: Метаданные для части контента, которую можно утвердить для развертывания.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 2e81fd688dde08522ff59322444b1c1cd0646054
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792136"
---
# <a name="catalogentry-resource-type"></a>тип ресурса catalogEntry

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Метаданные для части контента, которую можно утвердить для развертывания.

Все записи каталога существуют как один из следующих производных типов: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) и [qualityUpdateCatalogEntry.](../resources/windowsupdates-qualityupdatecatalogentry.md)

Базовый тип [для softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).

Это абстрактный тип.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|Дата, в которую контент больше не доступен для развертывания с помощью службы. Только для чтения.|
|displayName|String|Отображение имени контента. Только для чтения.|
|id|String|Уникальный идентификатор для записи каталога. Только для чтения.|
|releaseDateTime|DateTimeOffset|Дата выпуска контента. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

