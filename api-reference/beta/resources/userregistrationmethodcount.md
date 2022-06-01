---
title: Тип ресурса userRegistrationMethodCount
description: Число пользователей, зарегистрированных для метода проверки подлинности.
author: besiler
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: c505ea408599dbb7b0c6803d03b87b2586d6d0c3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820079"
---
# <a name="userregistrationmethodcount-resource-type"></a>Тип ресурса userRegistrationMethodCount

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Число пользователей, зарегистрированных для метода проверки подлинности.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|authenticationMethod|Строка|Имя метода проверки подлинности.|
|userCount|Int64|Число зарегистрированных пользователей.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodCount",
  "authenticationMethod": "String",
  "userCount": "Integer"
}
```
