---
title: тип ресурса microsoftAuthenticatorAuthenticationMethod
description: Представление приложения Microsoft Authenticator, зарегистрированного на пользователя. Microsoft Authenticator является методом проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 61f263b45b8e353622f06e6912f0659e2a8e147fabe208d8ea9ea2b94f555884
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54211943"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a>тип ресурса microsoftAuthenticatorAuthenticationMethod

Пространство имен: microsoft.graph

Представление приложения Microsoft Authenticator, зарегистрированного на пользователя. Microsoft Authenticator является методом проверки подлинности.

Наследует от [проверки подлинностиMethod](../resources/authenticationmethod.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список microsoftAuthenticatorAuthenticationMethods](../api/microsoftauthenticatorauthenticationmethod-list.md)|[коллекция microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)|Получите список объектов [MicrosoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) и их свойств.|
|[Get microsoftAuthenticatorAuthenticationMethod](../api/microsoftauthenticatorauthenticationmethod-get.md)|[MicrosoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)|Ознакомьтесь с свойствами и отношениями объекта [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)|
|[Удаление MicrosoftAuthenticatorAuthenticationMethod](../api/microsoftauthenticatorauthenticationmethod-delete.md)|Нет|Удаляет объект [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время регистрации этого приложения. Это свойство является null, если устройство не зарегистрировано для Телефон вход.|
|displayName|String|Имя устройства, на котором зарегистрировано это приложение.|
|id|String|Уникальный идентификатор для этого метода проверки подлинности. Унаследованный от [проверки подлинностиMethod](../resources/authenticationmethod.md)|
|deviceTag|String|Теги, содержащие метаданные приложений.|
|phoneAppVersion|String|Числовая версия этого экземпляра Authenticator приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|device;|[device](../resources/device.md)|Зарегистрированное устройство, на котором Microsoft Authenticator находится. Это свойство является null, если устройство не зарегистрировано для Телефон вход.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "deviceTag": "String",
  "phoneAppVersion": "String",
  "createdDateTime": "DateTimeOffset"
}
```
