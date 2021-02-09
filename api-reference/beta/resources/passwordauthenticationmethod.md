---
title: Тип ресурса passwordAuthenticationMethod
description: Представление пароля, зарегистрированного для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 92e135b74bc68662749376298b4be44155b577b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156695"
---
# <a name="passwordauthenticationmethod-resource-type"></a>Тип ресурса passwordAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление пароля пользователя. В целях безопасности сам пароль никогда не возвращается в объекте, но для сброса пароля можно принять меры.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Список passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | [Коллекция passwordAuthenticationMethod](passwordauthenticationmethod.md) | Чтение свойств и связей всех объектов **passwordAuthenticationMethod** этого пользователя. |
|[Get passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | Чтение свойств и связей объекта **passwordAuthenticationMethod.** |
|[Сброс пароля](../api/passwordauthenticationmethod-resetpassword.md)|Нет|Сброс пароля пользователя в облаке и, если он синхронизирован, в локальной сети.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|creationDateTime|DateTimeOffset|Дата и время последнего обновления пароля. Это свойство в настоящее время не заполнено. Только для чтения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Идентификатор этого пароля, зарегистрированного для этого пользователя. Только для чтения.|
|password|Строка|Для обеспечения безопасности пароль всегда возвращается в качестве NULL из операции LIST или GET.|

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


