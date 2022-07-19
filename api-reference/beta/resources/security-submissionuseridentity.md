---
title: Тип ресурса submissionUserIdentity
description: Представляет удостоверение пользователя, отправлявшего отправку угрозы.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c6f0fbd5c5f413200f358044a0bd202c0e4c031a
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856848"
---
# <a name="submissionuseridentity-resource-type"></a>Тип ресурса submissionUserIdentity

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удостоверение пользователя, отправлявшего отправку угрозы.

Наследуется от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание                                                                                                    |
|:------------|:-------|:---------------------------------------------------------------------------------------------------------------|
| displayName | Строка | Наследуется от **удостоверения**.                                                                 |
| email       | String | Адрес электронной почты пользователя, который выполняет отправку при входе в систему (делегированный вариант маркера). | 
| id          | String | Наследуется от **удостоверения**.  |


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionUserIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionUserIdentity",
  "displayName": "String",
  "id": "String (identifier)",
  "email": "String"
}
```

