---
title: Тип ресурса userRegistrationDetails
description: Представляет состояние методов проверки подлинности пользователя, включая, какие методы зарегистрированы и какие функции зарегистрированы и поддерживаются пользователем (например, многофакторная проверка подлинности, самостоятельный сброс пароля и проверка подлинности без пароля).
author: danielwood95
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8c2df96cd680896854866618c10a70aae3e65a37
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694730"
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
|id|String|Идентификатор объекта пользователя в Azure AD. Наследуется от [сущности](../resources/entity.md).|
|isMfaCapable|Логический|Указывает, зарегистрировал ли пользователь надежный метод проверки подлинности для многофакторной проверки подлинности. Метод должен быть разрешен политикой [методов проверки подлинности](../resources/authenticationmethodspolicy.md). Поддерживает `$filter` (`eq`).|
|isMfaRegistered|Логический|Указывает, зарегистрировал ли пользователь надежный метод проверки подлинности для многофакторной проверки подлинности. Этот метод не обязательно может быть разрешен политикой [методов проверки подлинности](../resources/authenticationmethodspolicy.md).  Поддерживает `$filter` (`eq`).|
|isPasswordlessCapable|Логический|Зарегистрирован ли пользователем метод строгой проверки подлинности без пароля (включая FIDO2, Windows Hello для бизнеса и Microsoft Authenticator (без пароля), разрешенный политикой методов проверки [подлинности](../resources/authenticationmethodspolicy.md). Поддерживает `$filter` (`eq`).|
|isSsprCapable|Логический|Указывает, зарегистрировал ли пользователь необходимое количество методов проверки подлинности для самостоятельного сброса пароля и разрешено ли пользователю выполнять самостоятельный сброс пароля политикой. Поддерживает `$filter` (`eq`).|
|isSsprEnabled|Логический|Разрешается ли пользователю выполнять самостоятельный сброс пароля по политике. Возможно, пользователь не обязательно зарегистрировал необходимое количество методов проверки подлинности для самостоятельного сброса пароля. Поддерживает `$filter` (`eq`).|
|isSsprRegistered|Логический|Указывает, зарегистрировал ли пользователь необходимое количество методов проверки подлинности для самостоятельного сброса пароля. Пользователю не обязательно разрешено выполнять самостоятельный сброс пароля по политике. Поддерживает `$filter` (`eq`).|
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

