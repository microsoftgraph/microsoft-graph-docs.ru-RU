---
title: тип ресурса attackSimulationUser
description: Пользователь в кампании моделирования атак и обучения.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 961a8af1bed831b019f41ddf6a7643ac3b26ab07
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979708"
---
# <a name="attacksimulationuser-resource-type"></a>тип ресурса attackSimulationUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пользователь в кампании моделирования атак и обучения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя пользователя.|
|email|String|Адрес электронной почты пользователя.|
|userId|String|Это свойство **id** для [](../resources/user.md) пользовательского ресурса, которое представляет пользователя в клиенте Azure AD.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationUser",
  "userId": "String",
  "displayName": "String",
  "email": "String"
}
```

