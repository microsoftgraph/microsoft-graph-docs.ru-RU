---
title: Тип ресурса phoneAuthenticationMethod
description: Представление телефона, зарегистрированного для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 397d55050cbe0e985075a83527efff45572afe0b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156688"
---
# <a name="phoneauthenticationmethod-resource-type"></a>Тип ресурса phoneAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление телефона, зарегистрированного для пользователя. Этот ресурс включает номер телефона, тип телефона и то, настроен ли для пользователя вход с помощью SMS.

Телефон имеет один из трех типов: мобильный, альтернативный мобильный телефон или офис. Пользователь может зарегистрировать один номер для каждого типа и должен иметь мобильный телефон до того, как будет добавлен альтернативный мобильный телефон. При использовании телефона для многофакторной проверки подлинности (MFA) или самостоятельного сброса пароля (SSPR) мобильный телефон используется по умолчанию, а альтернативный мобильный телефон является резервным. 

Мобильные телефоны можно использовать как для SMS-вызовов, так и для голосовых вызовов в зависимости от параметров клиента.

Офисный телефон может принимать только голосовые вызовы, а не SMS-сообщения.

Свойство состояния для входов в систему с помощью SMS-сообщения предоставляет сведения о готовности номера телефона к входу через SMS. Ниже возможен вариант значений.

|Значение|Описание|
|--------|-----------|
|`notSupported`|Основной вход не поддерживается для этого метода проверки подлинности. Например, вход можно включить только на основном мобильном номере пользователя, а не на альтернативном номере.|
|`notAllowedByPolicy`|Политика не позволяет этому пользователю использовать этот метод в качестве основного входа.|
|`notConfigured`|Политика позволяет этому пользователю использовать этот метод в качестве основного входа, но для его настройки необходимо принять дополнительные меры.|
|`phoneNumberNotUnique`|Этот пользователь попытался настроить номер телефона в качестве основного, но он не был уникальным и не может использоваться в качестве имени для регистрации.|
|`ready`|Этот метод проверки подлинности готов к использованию при основном входе.|

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/Authentication-list-phonemethods.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Чтение свойств и связей всех объектов phoneAuthenticationMethod этого пользователя. |
| [Получение](../api/phoneauthenticationmethod-get.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Чтение свойств и связей объекта phoneAuthenticationMethod. |
| [Обновление](../api/phoneauthenticationmethod-update.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Обновление объекта phoneAuthenticationMethod. |
| [удаление](../api/phoneauthenticationmethod-delete.md); | Нет | Удаление объекта phoneAuthenticationMethod. |
|[Отключение sms-подписи](../api/phoneauthenticationmethod-disablesmssignin.md)|Нет|Отключите вход с помощью SMS для пользователя.|
|[Включить вход с помощью SMS](../api/phoneauthenticationmethod-enablesmssignin.md)|Нет|Включит вход с помощью SMS для пользователя.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Идентификатор этого телефона, зарегистрированного для этого пользователя. Только для чтения.|
|phoneNumber|String|Номер телефона для текста или вызов для проверки подлинности. Номера телефонов используют формат "+ \<country code\> \<number\> \<extension\> x", с необязательным расширением. Например, допустимы +1 5555551234 или +1 5555551234x123. Числа отклоняется при создании или обновлении, если они не соответствуют требуемму формату. |
|phoneType|string|Тип этого телефона. Возможные значения: `mobile` , , или `alternateMobile` `office` .|
|smsSignInState|string|Можно ли использовать телефон для sms-входов. Возможные значения: `notSupported` , , , , , или `notAllowedByPolicy` `notEnabled` `phoneNumberNotUnique` `ready` `notConfigured` .|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "string",
  "smsSignInState": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


