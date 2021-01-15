---
title: Тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f2d5dbc64fe81b629f89cf0b98bd3f2d32c1411
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874497"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a>Тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности Microsoft Authenticator. Политики методов проверки подлинности определяют параметры конфигурации и пользователей или группы, которые могут использовать этот метод проверки подлинности.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[получение](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md);|[microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|Чтение свойств и связей объекта microsoftAuthenticatorAuthenticationMethodConfiguration.|
|[Обновление](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[microsoftAuthenticatorAuthenticationMethodConfiguration](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|Обновление свойств объекта microsoftAuthenticatorAuthenticationMethodConfiguration.|
|[удаление](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md);|Нет|Возвращает объект microsoftAuthenticatorAuthenticationMethodConfiguration в конфигурацию по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[Коллекция microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)|Коллекция пользователей или групп, которым включен метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

