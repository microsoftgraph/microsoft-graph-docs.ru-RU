---
title: Тип ресурса tenantAllowOrBlockListAction
description: Представляет действие списка разрешений или блокирования клиента
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 26dc913078122a1bbb994369e63e2e2c0336f6c0
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856921"
---
# <a name="tenantalloworblocklistaction-resource-type"></a>Тип ресурса tenantAllowOrBlockListAction

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие списка разрешений или блокирования клиента. Когда администратор создает отправку угроз по электронной почте, можно также указать операцию списка блокировки разрешений клиента. Если указана операция списка блокирования разрешений клиента, отправка угроз автоматически добавит связанные элементы (URL-адреса, вложения, отправители) в список разрешенных блоков клиента.

## <a name="properties"></a>Свойства
| Свойство           | Тип                                        | Описание                                                                      |
|:-------------------|:--------------------------------------------|:---------------------------------------------------------------------------------|
| action             | tenantAllowBlockListAction                  | Указывает, является ли список разрешенных блоков клиента разрешенным или блоком. Возможные значения: `allow`, `block` и `unkownFutureValue`.|
| expirationDateTime | DateTimeOffset                              | Указывает, когда срок действия списка разрешенных блоков клиента истекает в дату и время.  |
| Примечание               | String                                      | Указывает заметку, добавленную в список разрешений клиента, в формате строки. |
| results            | Collection([security.tenantAllowBlockListEntryResult](../resources/security-tenantallowblocklistentryresult.md)) | Содержит результат отправки, которая приводит к созданию записи списка разрешенных блоков клиента. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.tenantAllowOrBlockListAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.tenantAllowOrBlockListAction",
  "action": "String",
  "results": [
    {
      "@odata.type": "microsoft.graph.security.tenantAllowBlockListEntryResult"
    }
  ],
  "expirationDateTime": "String (timestamp)",
  "note": "String"
}
```

