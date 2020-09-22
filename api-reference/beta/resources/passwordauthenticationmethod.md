---
title: Тип ресурса Пассвордаусентикатионмесод
description: Представление пароля, зарегистрированного для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c61367520f9dccb47fe238a92366cefd41748865
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998231"
---
# <a name="passwordauthenticationmethod-resource-type"></a>Тип ресурса Пассвордаусентикатионмесод

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление пароля пользователя. В целях безопасности сам пароль никогда не возвращается в объекте, но для сброса пароля можно предпринять действие.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
|[Список Пассвордаусентикатионмесодс](../api/authentication-list-passwordmethods.md) | Коллекция [пассвордаусентикатионмесод](passwordauthenticationmethod.md) | Чтение свойств и связей всех объектов **пассвордаусентикатионмесод** этого пользователя. |
|[Получение Пассвордаусентикатионмесод](../api/passwordauthenticationmethod-get.md) | [пассвордаусентикатионмесод](passwordauthenticationmethod.md) | Чтение свойств и связей объекта **пассвордаусентикатионмесод** . |
|[Сброс пароля](../api/passwordauthenticationmethod-resetpassword.md)|Нет|Сброс пароля пользователя в облаке и, если синхронизация выполняется в локальной среде.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|креатиондатетиме|DateTimeOffset|Дата и время последнего обновления этого пароля. В настоящее время это свойство не заполняется. Только для чтения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|id|String| Идентификатор этого пароля, зарегистрированный для этого пользователя. Только для чтения.|
|password|Строка|В целях безопасности пароль всегда возвращается как NULL из списка или операции GET.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "baseType": "",
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


