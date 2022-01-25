---
title: тип ресурса userRegistrationDetails
description: Представляет состояние методов проверки подлинности пользователя, в том числе зарегистрированных методов и функций, на которые зарегистрирован и способен пользователь (например, многофакторная проверка подлинности, сброс пароля самообслуживления и проверка подлинности без паролей).
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 11d447b1b4c9069bd4c8d8c29271c4d0b6f51380
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201787"
---
# <a name="userregistrationdetails-resource-type"></a>тип ресурса userRegistrationDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние методов проверки подлинности пользователя, в том числе зарегистрированных методов и функций, на которые зарегистрирован и способен пользователь (например, многофакторная проверка подлинности, сброс пароля самообслуживления и проверка подлинности без паролей).

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список userRegistrationDetails](../api/authenticationmethodsroot-list-userregistrationdetails.md)|[коллекция userRegistrationDetails](../resources/userregistrationdetails.md)|Получите список объектов [userRegistrationDetails](../resources/userregistrationdetails.md) и их свойств.|
|[Get userRegistrationDetails](../api/userregistrationdetails-get.md)|[userRegistrationDetails](../resources/userregistrationdetails.md)|Ознакомьтесь с свойствами и отношениями [объекта userRegistrationDetails.](../resources/userregistrationdetails.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта пользователя в Azure AD. Наследуется от [сущности](../resources/entity.md).|
|isMfaCapable|Boolean|Зарегистрировал ли пользователь эффективный метод проверки подлинности для многофакторной проверки подлинности. Метод должен быть разрешен политикой методов [проверки подлинности.](../resources/authenticationmethodspolicy.md) Поддерживает `$filter` (`eq`).|
|isMfaRegistered|Boolean|Зарегистрировал ли пользователь эффективный метод проверки подлинности для многофакторной проверки подлинности. Метод не обязательно может быть разрешен политикой методов [проверки подлинности.](../resources/authenticationmethodspolicy.md)  Поддерживает `$filter` (`eq`).|
|isPasswordlessCapable|Boolean|Зарегистрировал ли пользователь надежный метод проверки подлинности без паролей (включая FIDO2, Windows Hello для бизнеса и Microsoft Authenticator (Passwordless)), разрешенный политикой методов проверки [подлинности.](../resources/authenticationmethodspolicy.md) Поддерживает `$filter` (`eq`).|
|isSsprCapable|Boolean|Зарегистрировано ли пользователем необходимое количество методов проверки подлинности для сброса пароля самообслуживаемой и разрешено ли пользователю выполнять сброс пароля самообслуживления политикой. Поддерживает `$filter` (`eq`).|
|isSsprEnabled|Boolean|Разрешено ли пользователю выполнять сброс пароля самообслуживки политикой. Возможно, пользователь не обязательно зарегистрировал необходимое количество методов проверки подлинности для сброса пароля самообслуживления. Поддерживает `$filter` (`eq`).|
|isSsprRegistered|Boolean|Зарегистрировал ли пользователь необходимое количество методов проверки подлинности для сброса пароля самообслуживления. Необязательно, чтобы пользователю было разрешено выполнять сброс пароля самообслуживки политикой. Поддерживает `$filter` (`eq`).|
|methodsRegistered|Коллекция объектов string|Коллекция зарегистрированных методов проверки подлинности, таких как `mobilePhone` `email` , `fido2` . Поддерживает `$filter` `any` (с `eq` ).|
|userDisplayName|String| Имя отображения пользователя, например `Adele Vance` . Поддерживает `$filter` `eq` (, `startsWith` ) и `$orderBy` .|
|userPrincipalName|String|Основное имя пользователя, например `AdeleV@contoso.com` . Поддерживает `$filter` `eq` (, `startsWith` ) и `$orderBy` .|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userRegistrationDetails",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationDetails",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "isMfaRegistered": "Boolean",
  "isMfaCapable": "Boolean",
  "isSsprRegistered": "Boolean",
  "isSsprEnabled": "Boolean",
  "isSsprCapable": "Boolean",
  "isPasswordlessCapable": "Boolean",
  "methodsRegistered": [
    "String"
  ]
}
```

