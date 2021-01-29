---
title: Тип ресурса userRegistrationFeatureSummary
description: Сводка пользователей, способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 3dc3b48e6883b8c953db5d7b826243989109f2d9
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052619"
---
# <a name="userregistrationfeaturesummary-resource-type"></a>Тип ресурса userRegistrationFeatureSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние того, сколько пользователей в организации могут выполнять многофакторную проверку подлинности, самостоятельный сброс паролей и проверку подлинности без пароля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [usersRegisteredByFeature](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | userRegistrationFeatureSummary | Получите количество пользователей, способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|totalUserCount|Int64|Общее количество учетных записей пользователей, за исключением заблокированных|
|userRegistrationFeatureCounts|[Коллекция userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md)|Количество пользователей, зарегистрированных или способных использовать многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.|
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
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationFeatureCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
    }
  ]
}
```
