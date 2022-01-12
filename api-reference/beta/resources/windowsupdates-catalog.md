---
title: Тип ресурса каталога
description: Объект, представляющий каталог контента, который можно утвердить для развертывания.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 0150875b940c9568212ae6a4acee0a0d01057feb
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863373"
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

