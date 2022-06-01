---
title: Тип ресурса userRegistrationMethodSummary
description: Сводка количества пользователей, зарегистрированных для каждого метода проверки подлинности.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e7c5288fb533f3b97ea5c69d7916e3cd3bc33d50
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820030"
---
# <a name="userregistrationmethodsummary-resource-type"></a>Тип ресурса userRegistrationMethodSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сводка количества пользователей, зарегистрированных для каждого метода проверки подлинности.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [usersRegisteredByMethod](../api/authenticationmethodsroot-usersregisteredbymethod.md) | userRegistrationMethodSummary | Получение числа пользователей, зарегистрированных для каждого метода проверки подлинности. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|totalUserCount|Int64|Общее число пользователей в клиенте.|
|userRegistrationMethodCounts|[Коллекция userRegistrationMethodCount](../resources/userregistrationmethodcount.md)|Число пользователей, зарегистрированных для каждого метода проверки подлинности.|
|userRoles|includedUserRoles|Тип роли пользователя. Возможные значения: `all`, `privilegedAdmin`, `admin`, `user`.|
|userTypes|includedUserTypes|Тип пользователя. Возможные значения: `all`, `member`, `guest`.|

Значение состоит `privilegedAdmin` из следующих привилегированных ролей администратора:

* Глобальный администратор
* Администратор безопасности
* Администратор условного доступа
* Администратор Exchange
* Администратор SharePoint
* Администратор службы поддержки
* Администратор выставления счетов
* Администратор пользователей
* Администратор проверки подлинности

Это значение включает `admin` все Azure AD роли администратора. 

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationMethodCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationMethodCount"
    }
  ]
}
```
