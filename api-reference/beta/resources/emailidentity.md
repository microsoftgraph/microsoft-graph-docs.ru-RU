---
title: Тип ресурса emailIdentity
description: Представляем удостоверение электронной почты пользователя.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 90882a78c149e089fd00baa266240cb574e9864a
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979755"
---
# <a name="emailidentity-resource-type"></a>Тип ресурса emailIdentity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляем удостоверение электронной почты пользователя.


Наследует от [удостоверения](../resources/identity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя пользователя. Унаследованный от [удостоверения](../resources/identity.md).|
|email|String|Адрес электронной почты пользователя.|
|id|String|ID пользователя. Унаследованный от [удостоверения](../resources/identity.md).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "email": "String"
}
```

