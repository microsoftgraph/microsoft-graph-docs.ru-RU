---
title: тип ресурса phoneAuthenticationMethod
description: Представление телефона, зарегистрированного на пользователя.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5a64e946973462995318b05993e85a09f919ead2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226311"
---
# <a name="phoneauthenticationmethod-resource-type"></a>тип ресурса phoneAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление телефона, зарегистрированного на пользователя. Этот ресурс включает номер телефона, тип телефона и настроен ли телефон, чтобы пользователь вошел с помощью SMS.

Телефон имеет один из трех типов: мобильный, альтернативный мобильный или офисный. Пользователь может иметь один номер, зарегистрированный для каждого типа, и должен иметь мобильный телефон перед добавлением альтернативного мобильного телефона. При использовании телефона для многофакторной проверки подлинности (MFA) или сброса пароля самообслуживления (SSPR) мобильный телефон является по умолчанию, а альтернативный мобильный телефон — резервное копирование. 

Мобильные телефоны можно использовать как для SMS, так и для голосовых вызовов в зависимости от параметров клиента.

Телефон в офисе может принимать только голосовые звонки, а не SMS-сообщения.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление](../api/authentication-list-phonemethods.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Чтение свойств и связей всех объектов phoneAuthenticationMethod этого пользователя. |
| [Получение](../api/phoneauthenticationmethod-get.md); | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Чтение свойств и связей объекта phoneAuthenticationMethod. |
| [Обновление](../api/phoneauthenticationmethod-update.md) | [phoneAuthenticationMethod](phoneauthenticationmethod.md) | Обновление объекта phoneAuthenticationMethod. |
| [удаление](../api/phoneauthenticationmethod-delete.md); | Нет | Удаление объекта phoneAuthenticationMethod. |
|[Отключение подписи SMS](../api/phoneauthenticationmethod-disablesmssignin.md)|Нет|Отключите вход в SMS для пользователя.|
|[Включить подписывку SMS](../api/phoneauthenticationmethod-enablesmssignin.md)|Нет|Включив вход в SMS для пользователя.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка| Идентификатор этого телефона, зарегистрированного для этого пользователя. Только для чтения. <br/><br/>Значение id является одним из следующих:<ul><li>`b6332ec1-7057-4abe-9331-3d72feddfe41` - где **phoneType** `alternateMobile` .</li><li>`e37fc753-ff3b-4958-9484-eaa9425c82bc` - где **phoneType** `office` .</li><li>`3179e48a-750b-4051-897c-87b9720928f7` - где **phoneType** `mobile` .</li>|
|phoneNumber|String|Номер телефона для текста или вызова для проверки подлинности. Телефон номера используют формат "+ \<country code\> \<number\> x \<extension\> ", с необязательным расширением. Например, допустимы +1 5555551234 или +1 555551234x1233. При создании и обновлении номера отклоняется, если они не соответствуют требуемой форме. |
|phoneType|проверка подлинностиPhoneType|Тип этого телефона. Возможные значения: `mobile`, `alternateMobile` или `office`.|
|smsSignInState|authenticationMethodSignInState|Готов ли телефон к входу в SMS или нет. Возможные значения: `notSupported` `notAllowedByPolicy` , , , , , `notEnabled` или `phoneNumberNotUnique` , `ready` `notConfigured` `unknownFutureValue` .|

### <a name="smssigninstate-values"></a>значения smsSignInState

Свойство государственного регистрации SMS дает сведения о том, готов ли номер телефона войти с помощью SMS. Ниже возможен вариант значений.

|Значение|Описание|
|--------|-----------|
|notSupported|Основной вход не поддерживается в этом методе проверки подлинности , например, вход можно включить только на основной мобильный номер пользователя, а не на альтернативном номере.|
|notAllowedByPolicy|Политика не позволяет этому пользователю использовать этот метод в качестве основного входа.|
|notConfigured|Политика позволяет этому пользователю использовать этот метод в качестве основного входа, но для его настройки необходимо принять дополнительные меры.|
|phoneNumberNotUnique|Этот пользователь попытался настроить номер телефона в качестве основного входного номера, но он не был уникальным и не может использоваться в качестве имени для регистрации.|
|готово|Этот метод проверки подлинности готов к использованию при первичном входе.|
|notEnabled|Этот метод входа не включен|

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


