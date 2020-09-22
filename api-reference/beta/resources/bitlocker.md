---
title: Тип BitLocker
description: Ресурс BitLocker
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ad8a05e82cd3f300bedf034fe18f67ce3359f16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038877"
---
# <a name="bitlocker-resource-type"></a>Тип ресурса BitLocker

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Родительский ресурс для сохраненного ключа BitLocker с помощью свойства навигации **битлоккеррековерикэй** , содержащего фактический ключ восстановления.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Рековерикэйс](../api/bitlocker-list-recoverykeys.md)|Коллекция [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md)|Получение списка объектов Битлоккеррековерикэй и их свойств.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип | Описание |
|--|--|--|
| рековерикэйс | Коллекция [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) | Ключи восстановления, связанные с сущностью BitLocker. |

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitlocker",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlocker"
}
```

