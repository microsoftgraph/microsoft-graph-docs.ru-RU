---
title: ресурс bitLocker
description: Родительский ресурс для сохраненного ключа BitLocker с свойством навигации bitlockerRecoveryKey, который содержит фактический ключ восстановления.
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ac73c0e7237f4d41217cb53c2c4c33d8cfcdb784
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689079"
---
# <a name="bitlocker-resource-type"></a>тип ресурса bitlocker

Пространство имен: microsoft.graph

Родительский ресурс для сохраненного ключа BitLocker с свойством навигации **bitlockerRecoveryKey,** который содержит фактический ключ восстановления.

## <a name="methods"></a>Методы
Нет.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип | Описание |
|--|--|--|
| recoveryKeys | [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection | Ключи восстановления, связанные с объектом bitlocker. |

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

