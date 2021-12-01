---
title: сложный тип singleUser
description: Определяет пользователя в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или рецензента.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9cc5549ef34fb9ee67a3337e0ba40bc38f413469
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242908"
---
# <a name="singleuser-complex-type"></a>сложный тип singleUser

Пространство имен: microsoft.graph

Используется в параметрах проверки запросов, утверждений и назначений политики назначения пакетов доступа. Это значение указывает на то, что этот userSet идентифицирует определенного пользователя в клиенте, которому будет разрешено в качестве запрашивателя, утверждения или  `@odata.type` `#microsoft.graph.singleUser` рецензента.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Имя пользователя в Azure AD. Только для чтения. |
|userId|String|ID пользователя [в](user.md) Azure AD.|

## <a name="relationships"></a>Связи
Отсутствуют.
## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.singleUser",
  "userId": "String",
  "description": "String"
}
```



