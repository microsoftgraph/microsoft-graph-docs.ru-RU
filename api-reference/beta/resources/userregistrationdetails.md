---
title: Тип ресурса userRegistrationDetails
description: Представляет состояние методов проверки подлинности пользователя, включая, какие методы зарегистрированы и какие функции зарегистрированы и поддерживаются пользователем (например, многофакторная проверка подлинности, самостоятельный сброс пароля и проверка подлинности без пароля).
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 55e3805de8619ef8e8b64f541b342991da6a44f7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820191"
---
# <a name="userregistrationdetails-resource-type"></a>Тип ресурса userRegistrationDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние методов проверки подлинности пользователя, включая, какие методы зарегистрированы и какие функции зарегистрированы и поддерживаются пользователем (например, многофакторная проверка подлинности, самостоятельный сброс пароля и проверка подлинности без пароля).

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление userRegistrationDetails](../api/authenticationmethodsroot-list-userregistrationdetails.md)|[Коллекция userRegistrationDetails](../resources/userregistrationdetails.md)|Получение списка объектов [userRegistrationDetails](../resources/userregistrationdetails.md) и их свойств.|
|[Получение userRegistrationDetails](../api/userregistrationdetails-get.md)|[userRegistrationDetails](../resources/userregistrationdetails.md)|Чтение свойств и связей объекта [userRegistrationDetails](../resources/userregistrationdetails.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultMfaMethod|defaultMfaMethodType|Метод, выбранный пользователем или администратором по умолчанию для выполнения многофакторной проверки подлинности для пользователя. Возможные значения: `none`, `mobilePhone`, `alternateMobilePhone`, `officePhone`, `microsoftAuthenticatorPush`, `softwareOneTimePasscode`, `unknownFutureValue`.|
|id|Строка|Идентификатор объекта пользователя в Azure AD. Наследуется от [сущности](../resources/entity.md).|
|isMfaCapable|Логическое|Указывает, зарегистрировал ли пользователь надежный метод проверки подлинности для многофакторной проверки подлинности. Метод должен быть разрешен политикой [методов проверки подлинности](../resources/authenticationmethodspolicy.md). Поддерживает `$filter` (`eq`).|
|isMfaRegistered|Логическое|Указывает, зарегистрировал ли пользователь надежный метод проверки подлинности для многофакторной проверки подлинности. Этот метод не обязательно может быть разрешен политикой [методов проверки подлинности](../resources/authenticationmethodspolicy.md).  Поддерживает `$filter` (`eq`).|
|isPasswordlessCapable|Логическое|Зарегистрирован ли пользователем метод строгой проверки подлинности без пароля (включая FIDO2, Windows Hello для бизнеса и Microsoft Authenticator (без пароля), разрешенный политикой методов проверки [подлинности](../resources/authenticationmethodspolicy.md). Поддерживает `$filter` (`eq`).|
|isSsprCapable|Логическое|Указывает, зарегистрировал ли пользователь необходимое количество методов проверки подлинности для самостоятельного сброса пароля и разрешено ли пользователю выполнять самостоятельный сброс пароля политикой. Поддерживает `$filter` (`eq`).|
|isSsprEnabled|Логическое|Разрешается ли пользователю выполнять самостоятельный сброс пароля по политике. Возможно, пользователь не обязательно зарегистрировал необходимое количество методов проверки подлинности для самостоятельного сброса пароля. Поддерживает `$filter` (`eq`).|
|isSsprRegistered|Логическое|Указывает, зарегистрировал ли пользователь необходимое количество методов проверки подлинности для самостоятельного сброса пароля. Пользователю не обязательно разрешено выполнять самостоятельный сброс пароля по политике. Поддерживает `$filter` (`eq`).|
|methodsRegistered|Коллекция String|Коллекция зарегистрированных методов проверки подлинности, таких как `mobilePhone`, `email`, . `fido2` Поддерживает ( `$filter` с`any` `eq`).|
|userDisplayName|String| Отображаемое имя пользователя, например `Adele Vance`. `$filter` Поддерживает (`eq`,`startsWith`) и `$orderBy`.|
|userPrincipalName|String|Имя участника-пользователя, например `AdeleV@contoso.com`. `$filter` Поддерживает (`eq`,`startsWith`) и `$orderBy`.|

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
  "defaultMethod": "String",
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

