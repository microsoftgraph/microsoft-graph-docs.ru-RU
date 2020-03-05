---
title: сложный тип Коннектедорганизатионмемберс
description: Тип Коннектедорганизатионмемберс определяет коллекцию пользователей в клиенте, которые будут разрешены в качестве запрашивающего, утверждающего или проверяющего.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20f4477998547d6e98572fd8409f69e811c2198d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507494"
---
# <a name="connectedorganizationmembers-complex-type"></a>сложный тип Коннектедорганизатионмемберс

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах запроса [политики назначения пакетов Access](accesspackageassignmentpolicy.md). `@odata.type` Значение `#microsoft.graph.connectedOrganizationMembers` указывает на то, что этот тип определяет коллекцию пользователей, которые связаны с подключенной Организацией и могут запрашивать пакет Access.

## <a name="properties"></a>Свойства

Этот тип имеет следующие свойства:

| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| id |Строка | Идентификатор подключенной Организации в управлении обслуживанием. |
| description |String | Имя подключенной Организации. Только для чтения. |
| Создание резервной копии | Логический | Не используется в данный момент. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено представление типа в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
  "isBackup": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
