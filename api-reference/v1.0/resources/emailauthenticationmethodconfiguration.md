---
title: тип ресурса emailAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности OTP электронной почты
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 99e4f642db1bc49c2717a4d2a262dbba5943b4c7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964947"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a>тип ресурса emailAuthenticationMethodConfiguration

Пространство имен: microsoft.graph

Представляет политику методов проверки подлинности электронной почты этого клиента. Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которым включен метод проверки подлинности. OTP-адрес электронной почты может использоваться облачными пользователями клиента для сброса пароля самообслуживления или внешними пользователями для проверки подлинности в некоторых случаях.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-get.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|Ознакомьтесь с свойствами и отношениями объекта emailAuthenticationMethodConfiguration.|
|[Обновление emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-update.md)|[emailAuthenticationMethodConfiguration](../resources/emailauthenticationmethodconfiguration.md)|Обновление свойств объекта emailAuthenticationMethodConfiguration.|
|[Удаление emailAuthenticationMethodConfiguration](../api/emailauthenticationmethodconfiguration-delete.md)|Нет|Удаляет объект emailAuthenticationMethodConfiguration.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности. Унаследованный от [проверки подлинностиMethodConfiguration](../resources/authenticationmethodconfiguration.md).|
|state|authenticationMethodState|Указывает, включен этот метод проверки подлинности или нет. Возможные значения: `enabled`, `disabled`.|
|allowExternalIdToUseEmailOtp|externalEmailOtpState|Определяет, является ли OTP электронной почты для внешних пользователей для проверки подлинности. Возможные значения: `default`, `enabled`, `disabled`, `unknownFutureValue`. Клиенты в состоянии, которое не использует общедоступный предварительный просмотр, автоматически будут иметь включенную OTP-почту начиная с `default` марта 2021 г.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "allowExternalIdToUseEmailOtp": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
