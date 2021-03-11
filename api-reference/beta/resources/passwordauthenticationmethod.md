---
title: passwordAuthenticationMethod resource type
description: Представление пароля, зарегистрированного пользователю.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f902d47d0d06857537a07541456596c3a6204bc3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720580"
---
# <a name="passwordauthenticationmethod-resource-type"></a>passwordAuthenticationMethod resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление пароля пользователя. Для безопасности сам пароль никогда не будет возвращен в объекте, но можно принять меры для сброса пароля.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Список passwordAuthenticationMethods](../api/authentication-list-passwordmethods.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) collection | Ознакомьтесь с свойствами и отношениями всех объектов **passwordAuthenticationMethod.** |
|[Get passwordAuthenticationMethod](../api/passwordauthenticationmethod-get.md) | [passwordAuthenticationMethod](passwordauthenticationmethod.md) | Ознакомьтесь с свойствами и отношениями объекта **passwordAuthenticationMethod.** |
|[Сброс пароля](../api/passwordauthenticationmethod-resetpassword.md)|Нет|Сброс пароля пользователя в облаке и при синхронизации с локальной.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|creationDateTime|DateTimeOffset|Дата и время последнего обновления пароля. Это свойство в настоящее время не заполнено. Только для чтения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String| Идентификатор этого пароля, зарегистрированного для этого пользователя. Только для чтения.|
|password|Строка|Для обеспечения безопасности пароль всегда возвращается в качестве null из операции LIST или GET.|

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


