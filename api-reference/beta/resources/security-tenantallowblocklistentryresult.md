---
title: Тип ресурса tenantAllowBlockListEntryResult
description: Представляет результат записи списка блокирования клиента.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9e5a92fbc215c814ce2f55a1e9a16407bc60f147
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856890"
---
# <a name="tenantallowblocklistentryresult-resource-type"></a>Тип ресурса tenantAllowBlockListEntryResult

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет результат записи списка разрешенных блоков клиента. Запись для элемента списка блокировки разрешений клиента может быть URL-адресом, вложением или отправителями.

## <a name="properties"></a>Свойства
| Свойство           | Тип                          | Описание                                             |
|:-------------------|:------------------------------|:--------------------------------------------------------|
| entryType          | tenantAllowBlockListEntryType | Тип записи списка блокирования разрешений клиента. Возможные значения: `url`, `fileHash`, и `sender``recipient` `unkownFutureValue`.  |
| expirationDateTime | DateTimeOffset                | Указывает, когда срок действия этой записи истекает по дате. |
| Идентичности           | Строка                        | Указывает удостоверение записи, созданной системой списка разрешенных блоков клиента. |
| status             | longRunningOperationStatus    | Указывает, успешно ли выполнена операция создания записи списка блокировки для клиента. Возможные значения: , , , , и `failed``skipped` `unkownFutureValue`. `succeeded``running``notStarted` |
| value              | String                        | Указывает значение записи списка разрешенных блоков созданного клиента.  |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.tenantAllowBlockListEntryResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.tenantAllowBlockListEntryResult",
  "identity": "String",
  "value": "String",
  "entryType": "String",
  "expirationDateTime": "String (timestamp)",
  "status": "String"
}
```

