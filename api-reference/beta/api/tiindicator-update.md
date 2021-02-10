---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3ded1ad2ac77cfd08320c54480de5dd24d319b91
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176957"
---
# <a name="update-tiindicator"></a>Обновление объекта tiIndicator

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [tiIndicator.](../resources/tiindicator.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | ThreatIndicators.ReadWrite.OwnedBy |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {code} **Required** |
|Prefer | return=representation |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились. Необходимые поля: `id` , `expirationDateTime` , `targetProduct` .

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|action|string| Действие, применяемая при совпадении индикатора из средства безопасности targetProduct. Возможные значения: `unknown`, `allow`, `block`, `alert`.|
|activityGroupNames|Коллекция String|Имена аналитики киберугроз для сторон, ответственных за вредоносные действия, на которые распространяется индикатор угроз.|
|additionalInformation|String|Область catchall, в которую могут быть помещены дополнительные данные индикатора, не охваченные другими свойствами tiIndicator. Данные, помещенные в additionalInformation, как правило, не используются средством безопасности targetProduct.|
|confidence|Int32|Integer representing the confidence the data within the indicator accurately identifies malicious behavior. Допустимые значения: 0–100, 100 — наивысшее.|
|description|String|Краткое описание (не более 100 символов) угрозы, представляемой индикатором.|
|diamondModel|[diamondModel](../resources/tiindicator.md#diamondmodel-values)|Область диамантской модели, в которой существует этот индикатор. Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Строка даты и времени, указывающая, когда истекает срок действия индикатора. Все индикаторы должны иметь дату окончания срока действия, чтобы избежать сохраняющихся устаревших индикаторов в системе. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|externalId|String|Идентификационный номер, который связывает индикатор с системой поставщика индикаторов (например, с внешней клавишей).|
|isActive|Логическое|Используется для отключения индикаторов в системе. По умолчанию любой отправленный индикатор является активным. Однако поставщики могут отправлять существующие индикаторы с этим набором "False", чтобы деактивировать индикаторы в системе.|
|killChain|[Коллекция killChain](../resources/tiindicator.md#killchain-values)|Массив строк JSON, который описывает точку или точку в цепочке событий, на которую направлен этот индикатор. Точные значения см. ниже в "killChain values".|
|knownFalsePositives|String|Сценарии, в которых индикатор может вызывать ложные срабатываия. Это должен быть текст, читаемый человеком.|
|lastReportedDateTime|DateTimeOffset|Время последнего увидеть индикатор. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|malwareFamilyNames|Коллекция String|Имя семейства вредоносных программ, связанное с индикатором, если оно существует. Корпорация Майкрософт по возможности предпочитает имя семейства вредоносных программ Майкрософт, которое можно найти с помощью Защитник Windows аналитики [безопасности.](https://www.microsoft.com/wdsi/threats)|
|passiveOnly|Логическое|Определяет, должен ли индикатор вызывать событие, которое видно конечному пользователю. Если установлено "true", средства безопасности не будут уведомлять конечного пользователя о том, что произошло "попадание". Это чаще всего рассматривается как аудит или режим в тихом режиме продуктами безопасности, в которых они просто регистрировали совпадение, но не выполняли это действие. Значение по умолчанию − ложь.|
|severity|Int32|Integer representing the severity of the malicious behavior identified by the data within the indicator. Допустимые значения: 0–5, где 5 — самый серьезный, а ноль — нет. Значение по умолчанию: 3.|
|tags|Коллекция String|Массив строк JSON, который хранит произвольные теги и ключевые слова.|
|tlpLevel|[tlpLevel](../resources/tiindicator.md#tlplevel-values)| Значение протокола light traffic light для индикатора. Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется необязательный заголовщик запроса, метод возвращает код отклика и обновленный объект `200 OK` [tiIndicator](../resources/tiindicator.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-request-without-prefer-header"></a>Пример 1. Запрос без загона Prefer

#### <a name="request"></a>Запрос

Ниже приводится пример запроса без `Prefer` загона.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Пример 2. Запрос с заголбом Prefer

#### <a name="request"></a>Запрос

Ниже приводится пример запроса, включаемого в `Prefer` заголок.

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> [!NOTE]
> Показанный здесь объект ответа может быть сокращен для учитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


