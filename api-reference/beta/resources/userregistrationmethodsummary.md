---
title: Тип ресурса userRegistrationMethodSummary
description: Сводка количества пользователей, зарегистрированных для каждого метода проверки подлинности.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 4f4d391291008bcbca1d017360bcb8caf3aea067
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052622"
---
# <a name="userregistrationmethodsummary-resource-type"></a>Тип ресурса userRegistrationMethodSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сводка количества пользователей, зарегистрированных для каждого метода проверки подлинности.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [usersRegisteredByMethod](../api/authenticationmethodsroot-usersregisteredbymethod.md) | userRegistrationMethodSummary | Получите количество пользователей, зарегистрированных для каждого метода проверки подлинности. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|totalUserCount|Int64|Общее количество пользователей в клиенте.|
|userRegistrationMethodCounts|[Коллекция userRegistrationMethodCount](../resources/userregistrationmethodcount.md)|Количество пользователей, зарегистрированных для каждого метода проверки подлинности.|
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

Значение включает `admin` все роли администратора Azure AD. 

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