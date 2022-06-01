---
title: Тип ресурса userRegistrationFeatureSummary
description: Сводка пользователей, способных выполнять многофакторную проверку подлинности, Self-Service сброс пароля и проверку подлинности без пароля.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b058276eaa3bc9f12dbe46ddc33afbe06b0bc2f2
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820149"
---
# <a name="userregistrationfeaturesummary-resource-type"></a>Тип ресурса userRegistrationFeatureSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние количества пользователей в организации, способных выполнять многофакторную проверку подлинности, самостоятельный сброс пароля и проверку подлинности без пароля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [usersRegisteredByFeature](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | userRegistrationFeatureSummary | Получение количества пользователей, способных выполнять многофакторную проверку подлинности, Self-Service сброс пароля и проверку подлинности без пароля. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|totalUserCount|Int64|Общее количество учетных записей пользователей, за исключением заблокированных|
|userRegistrationFeatureCounts|[Коллекция userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md)|Число пользователей, зарегистрированных или поддерживающих многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.|
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
