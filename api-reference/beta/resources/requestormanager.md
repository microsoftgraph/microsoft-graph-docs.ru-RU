---
title: сложный тип requestorManager
description: Определяет отношение к другому пользователю в клиенте, которому будет разрешено в качестве утвержденного.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4bfd42854a55ec2daa9e380c539a25479b0e933
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761081"
---
# <a name="requestormanager-complex-type"></a>сложный тип requestorManager

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используется в параметрах утверждения политики назначения [пакета доступа.](accesspackageassignmentpolicy.md) Это подтип [userSet,](userset.md)в котором значение указывает, что администратор запрашиваемого пользователя должен `@odata.type` `#microsoft.graph.requestorManager` быть одобрением.  При создании этапа утверждения политики назначения пакетов доступа с помощью requestorManager также включаем другого участника, например одного пользователя или члена группы, в случае, если у запрашиваемого пользователя нет менеджера.


## <a name="properties"></a>Свойства


| Свойство                     | Тип                      | Описание |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Для диспетчера на стадии утверждения указывает, является ли он резервным утверждением резервного копирования. |
|managerLevel | Int32 | Иерархический уровень руководителя в отношении запросителя. Например, у непосредственного менеджера запросителя будет managerLevel 1, а у менеджера менеджера запросителя будет managerLevel 2. Значение по умолчанию для managerLevel — 1. Возможные значения для этого свойства варьируются от 1 до 2. |


## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON этого типа.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "managerLevel": 1
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


