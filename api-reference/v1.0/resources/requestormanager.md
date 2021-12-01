---
title: сложный тип requestorManager
description: Определяет отношение к другому пользователю в клиенте, которому будет разрешено в качестве утвержденного.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a4f82b55438fe2e077cca299d55aa6af2c0fecb
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242968"
---
# <a name="requestormanager-complex-type"></a>сложный тип requestorManager

Пространство имен: microsoft.graph

Используется в параметрах утверждения политики назначения пакета доступа.
Это подтип [subjectSet,](subjectset.md)в котором значение указывает, что администратор запрашиваемого пользователя должен `@odata.type` `#microsoft.graph.requestorManager` быть одобрением.  При создании этапа утверждения политики назначения пакетов доступа с помощью requestorManager также включаем другого участника, например одного пользователя или члена группы, в случае, если у запрашиваемого пользователя нет менеджера.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|managerLevel|Int32|Иерархический уровень руководителя в отношении запросителя. Например, у непосредственного менеджера запросителя будет managerLevel 1, а у менеджера менеджера запросителя будет managerLevel 2. Значение по умолчанию для managerLevel — 1. Возможные значения для этого свойства варьируются от 1 до 2. |

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestorManager",
  "managerLevel": "Integer"
}
```


