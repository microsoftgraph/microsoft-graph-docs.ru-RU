---
title: Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности на телефоне без пароля Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e27424264293d87775937c7893546ec321728b4a
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872284"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type-deprecated"></a>Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration (неподдерживаем)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности на телефоне без пароля Microsoft Authenticator. Политики методов проверки подлинности определяют параметры конфигурации и пользователей или группы, которые могут использовать этот метод проверки подлинности.

> [!CAUTION]
> API политики проверки подлинности для телефона без пароля Microsoft Authenticator является неподготовленным и больше не возвращает результаты 31 декабря 2020 г. Используйте новую политику метода [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md) (неподготовлен)|[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Чтение свойств и связей объекта без пароляMicrosoftAuthenticatorAuthenticationMethodConfiguration.|
|[Обновление](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md) (неподготовлено) |[passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Обновление свойств объекта passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.|
|[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md) (deprecated)|Нет|Возвращает объект passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration в конфигурацию по умолчанию.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[Коллекция passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md)|Коллекция пользователей или групп, которым включен метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
