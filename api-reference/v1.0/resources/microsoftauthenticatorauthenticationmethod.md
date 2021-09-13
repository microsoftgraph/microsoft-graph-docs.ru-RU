---
title: тип ресурса microsoftAuthenticatorAuthenticationMethod
description: Представление приложения Microsoft Authenticator, зарегистрированного на пользователя. Microsoft Authenticator является методом проверки подлинности.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ea3614af67720c9c35a641a3f6729eabf98d5dd8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134502"
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
|displayName|Строка|Имя устройства, на котором зарегистрировано это приложение.|
|id|Строка|Уникальный идентификатор для этого метода проверки подлинности. Унаследованный от [проверки подлинностиMethod](../resources/authenticationmethod.md)|
|deviceTag|String|Теги, содержащие метаданные приложений.|
|phoneAppVersion|Строка|Числовая версия этого экземпляра Authenticator приложения.|

## <a name="relationships"></a>Отношения
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
