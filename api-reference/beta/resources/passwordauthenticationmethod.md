---
title: passwordAuthenticationMethod resource type
description: Представление пароля, зарегистрированного пользователю.
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 196964495c93a6d9dcdd35e58803500abee9c4a7
ms.sourcegitcommit: dab085b74666e190974a35e6a124d3ff1645fa25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2022
ms.locfileid: "64646580"
---
# <a name="passwordauthenticationmethod-resource-type"></a>passwordAuthenticationMethod resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление пароля пользователя. Для безопасности сам пароль никогда не будет возвращен в объекте, но можно принять меры для сброса пароля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Список passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) collection | Ознакомьтесь с свойствами и отношениями всех объектов **passwordAuthenticationMethod** . |
|[Get passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | Ознакомьтесь с свойствами и отношениями объекта **passwordAuthenticationMethod** . |
|[Сброс пароля](../api/passwordauthenticationmethod-resetpassword.md)|Никаких других изменений не происходит|Сброс пароля пользователя в облаке и при синхронизации с локальной.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|creationDateTime|DateTimeOffset|Дата и время последнего обновления пароля. Это свойство в настоящее время не заполнено. Только для чтения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String| Идентификатор этого пароля, зарегистрированного для этого пользователя. Это обычно `28c10230-6103-485e-b985-444c60001490`. Только для чтения.|
|password|Строка|Для обеспечения безопасности пароль всегда возвращается с `null` помощью операции LIST или GET.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "creationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "password": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


