---
title: Тип ресурса Усеркредентиалусажедетаилс
description: Представляет использование функции самостоятельного сброса пароля для данного клиента.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 9ff48554c7bab011171136181c7a1ab0ce8b01db
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384984"
---
# <a name="usercredentialusagedetails-resource-type"></a>Тип ресурса Усеркредентиалусажедетаилс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет использование функции самостоятельного сброса пароля для данного клиента. Сведения включают сведения о пользователе, состояние сброса и причину сбоя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Усеркредентиалусажедетаилс](../api/reportroot-list-usercredentialusagedetails.md) | усеркредентиалусажедетаилс | Чтение свойств и связей объекта Усеркредентиалусажедетаилс. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| аусмесод | string | Представляет способ проверки подлинности, используемый пользователем. Возможные значения `email`:, `mobileSMS`, `mobileCall` `officePhone`,, `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode`и `alternateMobileCall` (поддерживается только при регистрации). |
| eventDateTime | DateTimeOffset | Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. |
| failureReason | String | Предоставляет причину ошибки для соответствующего сброса или рабочего процесса регистрации. |
| состав | string | Возможные значения: `registration` и `reset`. |
| id | String | Только для чтения. Уникальный идентификатор действия. Только для чтения.|
| Выполнение | Boolean | Указывает на успешное или неудачное завершение рабочего процесса. |
| userDisplayName | String | Имя пользователя, выполняющего сброс или регистрацию рабочего процесса. |
| userPrincipalName | Строка | Имя участника-пользователя, выполняющего сброс или регистрацию. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->