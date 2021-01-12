---
title: Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Представление метода входов на телефоне без пароля Microsoft Authenticator, зарегистрированного для пользователя.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8815d84a8a85491399e97f7d10aa2e6cc1aeaf9d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796551"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type-deprecated"></a>Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethod (неподготовлен)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление метода входов на телефон без пароля Microsoft Authenticator, зарегистрированного для пользователя.

> [!CAUTION]
> API метода microsoft Authenticator Без пароля для телефона является неподготовленным и перестает возвращать результаты 31 декабря 2020 г. Используйте новый метод [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (неподготовлен)|[Коллекция passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Получить список объектов без пароля ПользователяMicrosoftAuthenticatorAuthenticationMethod и их свойств.|
|[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (неподготовлен)|[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Чтение свойств и связей объекта user без пароляMicrosoftAuthenticatorAuthenticationMethod.|
|[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (deprecated)|Нет|Удаляет объект user без пароляMicrosoftAuthenticatorAuthenticationMethod.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор метода проверки подлинности.|
|displayName|String|Отображаемое имя мобильного устройства, заданное пользователем.|
|creationDateTime|DateTimeOffset|Временная пометь, когда этот метод был зарегистрирован для пользователя.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

