---
title: тип ресурса acl
description: Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 339b5ab51fd604cae2dd42e2ec853ede8d27ef5b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467832"
---
# <a name="acl-resource-type"></a>тип ресурса acl

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) [externalConnection.](externalconnectors-externalconnection.md)

## <a name="properties"></a>Свойства

| Свойство       | Тип   | Описание                                        |
|:---------------|:-------|:---------------------------------------------------|
| accessType     | String | Доступ, предоставленный удостоверению. Возможные значения: `grant`, `deny`. |
| identitySource | String | Источник удостоверений. Возможные значения: `azureActiveDirectory` или `external`.           |
| type           | String | Тип удостоверения. Возможные значения: , , если identitySource есть и только `user` если `group` `everyone` `everyoneExceptGuests` `azureActiveDirectory` `group` identitySource `external` является . |
| value          | String | Уникальный идентификатор удостоверения. В случае Azure Active Directory удостоверений устанавливается идентификатор объекта пользователя, группы или клиента для пользователей, групп и всех `value` (и всех пользователейExceptGuests) соответственно. В случае внешних `value` групп задают ID [externalGroup](externalconnectors-externalgroup.md).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
