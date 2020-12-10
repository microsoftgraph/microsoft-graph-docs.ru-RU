---
title: Тип ресурса Емаилаусентикатионмесодконфигуратион
description: Представляет политику методов проверки подлинности методом проверки подлинности методом OTP
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e3e18973759d7f120dd0bd8e984c98568054960
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617145"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a>Тип ресурса Емаилаусентикатионмесодконфигуратион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности методом проверки подлинности OTP для этого клиента. Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или группы, для которых разрешено использование метода проверки подлинности. В некоторых случаях для проверки подлинности с помощью облачных пользователей для самостоятельного сброса пароля или внешними пользователями для проверки подлинности может использоваться подтверждение подлинности OTP.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение Емаилаусентикатионмесодконфигуратион](../api/emailauthenticationmethodconfiguration-get.md)|[емаилаусентикатионмесодконфигуратион](../resources/emailauthenticationmethodconfiguration.md)|Чтение свойств и связей объекта Емаилаусентикатионмесодконфигуратион.|
|[Обновление Емаилаусентикатионмесодконфигуратион](../api/emailauthenticationmethodconfiguration-update.md)|[емаилаусентикатионмесодконфигуратион](../resources/emailauthenticationmethodconfiguration.md)|Обновление свойств объекта Емаилаусентикатионмесодконфигуратион.|
|[Удаление Емаилаусентикатионмесодконфигуратион](../api/emailauthenticationmethodconfiguration-delete.md)|Нет|Удаляет объект Емаилаусентикатионмесодконфигуратион.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности. Наследуется от [аусентикатионмесодконфигуратион](../resources/authenticationmethodconfiguration.md).|
|state|аусентикатионмесодстате|Указывает, включен ли этот метод проверки подлинности. Возможные значения: `enabled`, `disabled`.|
|алловекстерналидтаусимаилотп|екстерналемаилотпстате|Определяет, будут ли для проверки подлинности использоваться внешние пользователи для проверки подлинности методом OTP. Возможные значения: `default`, `enabled`, `disabled`, `unknownFutureValue`. Клиенты, для `default` которых не использовалась общедоступная Предварительная версия, автоматически включили OTP, начиная с 2021 марта.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|инклудетаржетс|Коллекция [аусентикатионмесодтаржет](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которым разрешено использовать метод проверки подлинности.|

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
