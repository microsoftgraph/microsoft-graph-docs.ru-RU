---
title: тип ресурса microsoftAuthenticatorAuthenticationMethod
description: Представление приложения Microsoft Authenticator, зарегистрированного для пользователя. Microsoft Authenticator — это метод проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aeb2d1d7b111c9424da2f927dbaf3030a356c6b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964827"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a>тип ресурса microsoftAuthenticatorAuthenticationMethod

Пространство имен: microsoft.graph

Представление приложения Microsoft Authenticator, зарегистрированного для пользователя. Microsoft Authenticator — это метод проверки подлинности.

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
|createdDateTime|DateTimeOffset|Дата и время регистрации этого приложения. Это свойство является нулевым, если устройство не зарегистрировано для без пароля.|
|displayName|String|Имя устройства, на котором зарегистрировано это приложение.|
|id|String|Уникальный идентификатор для этого метода проверки подлинности. Унаследованный от [проверки подлинностиMethod](../resources/authenticationmethod.md)|
|deviceTag|String|Теги, содержащие метаданные приложений.|
|phoneAppVersion|String|Числовая версия этого экземпляра приложения Authenticator.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|device;|[device](../resources/device.md)|Зарегистрированное устройство, на котором находится Microsoft Authenticator. Это свойство является нулевым, если устройство не зарегистрировано для без пароля.|

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
