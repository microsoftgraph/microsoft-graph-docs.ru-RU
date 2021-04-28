---
title: Тип ресурса каталога
description: Объект, представляющий каталог контента, который можно утвердить для развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3fc0630a36d123e6c3e208838d81ee7c33c62853
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068215"
---
# <a name="catalog-resource-type"></a>Тип ресурса каталога

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект, представляющий каталог контента, который можно утвердить для развертывания.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Записи списка](../api/windowsupdates-catalog-list-entries.md)|[коллекция microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md)|Получите ресурсы [catalogEntry](../resources/windowsupdates-catalogentry.md) из свойства навигации записей. Возвращает **ресурсы catalogEntry** следующих производных типов: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор каталога. Только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|записи|[коллекция microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md)|Списки содержимого, которое можно утвердить для развертывания. Только для чтения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalog",
  "id": "String (identifier)"
}
```

