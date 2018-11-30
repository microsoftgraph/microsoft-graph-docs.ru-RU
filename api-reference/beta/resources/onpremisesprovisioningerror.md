---
title: Тип ресурса onPremisesProvisioningError
description: Представляет ошибок синхронизации службы каталогов для пользователя, группы или организационной сущностей для контактов, при синхронизации локальных каталогов в Azure Active Directory.
ms.openlocfilehash: 9fa7850d39c9f7a490135a127938fc7fae30b6f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077456"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Тип ресурса onPremisesProvisioningError

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ошибок синхронизации службы каталогов для объектов [пользователей](user.md), [группы](group.md)или [организации контакта](orgcontact.md) при синхронизации локальных каталогов в Azure Active Directory.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|category|String| Категория Ошибка подготовки. Примечание: В настоящее время доступно только один значений. Возможные значения: *PropertyConflict* - указывает значение свойства не является уникальным. Такое же значение для свойства содержат другие объекты. |
|occurredDateTime|DateTimeOffset| Дата и время, в котором возникла ошибка. |
|propertyCausingError|String| Имя свойства каталогов, вызывает ошибку. Текущий возможные значения: *UserPrincipalName* или *ProxyAddress* |
|value|String| Значение свойства, вызывая ошибки. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->