---
title: Обновление объекта tiIndicator
description: Обновление свойств объекта tiIndicator.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: d3e4c65971ad240e5b8ede46a7562f102a4c8ece
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115573"
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
| Приложение                            | ThreatIndicators.ReadWrite.OwnedBy |

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

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились. Необходимые поля: `id` , `expirationDateTime` `targetProduct` .

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|action|string| Действие, применяемая, если индикатор соответствует из средства безопасности targetProduct. Возможные значения: `unknown`, `allow`, `block`, `alert`.|
|activityGroupNames|Коллекция строк|Имя разведки киберугроз для сторон, ответственных за вредоносную деятельность, подпадаемую под индикатор угрозы.|
|additionalInformation|Строка|Область catchall, в которую могут быть помещены дополнительные данные из индикатора, не охваченного другими свойствами tiIndicator. Данные, помещенные в дополнительнуюinformation, как правило, не будут использоваться средством безопасности targetProduct.|
|confidence|Int32|Integer, представляющий доверие к данным в индикаторе, точно определяет вредоносное поведение. Допустимые значения : 0 — 100, а 100 — самые высокие.|
|description|Строка|Краткое описание (100 символов или менее) угрозы, представленной индикатором.|
|diamondModel|[diamondModel](../resources/tiindicator.md#diamondmodel-values)|Область бриллиантовой модели, в которой существует этот индикатор. Возможные значения: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| Строка DateTime, указывающая, когда истекает срок действия индикатора. Чтобы избежать сохраняющихся в системе устаревших индикаторов, все индикаторы должны иметь дату истечения срока действия. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|externalId|String|Идентификационный номер, который связывает индикатор с системой поставщика индикаторов (например, с иностранным ключом).|
|isActive|Логический|Используется для отключения индикаторов внутри системы. По умолчанию любой представленный индикатор задан как активный. Однако для отключения индикаторов в системе поставщики могут отправлять существующие индикаторы с этим набором в "False".|
|killChain|[коллекция killChain](../resources/tiindicator.md#killchain-values)|Массив строк JSON, который описывает, какие точки или точки на цепочке убийств этот индикатор цели. Для точных значений см. ниже "killChain values".|
|knownFalsePositives|Строка|Сценарии, в которых индикатор может вызывать ложные срабатыва- Это должен быть текст, читаемый для человека.|
|lastReportedDateTime|DateTimeOffset|Последний раз индикатор был замечен. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|malwareFamilyNames|Коллекция строк|Семейство вредоносных программ, связанное с индикатором, если оно существует. Корпорация Майкрософт предпочитает семейство вредоносных программ Майкрософт, если это возможно, которое можно найти в энциклопедии угрозы Защитник Windows security [Intelligence](https://www.microsoft.com/wdsi/threats).|
|passiveOnly|Логический|Определяет, должен ли индикатор вызвать событие, которое видно конечному пользователю. При наборе "true" средства безопасности не будут уведомлять конечного пользователя о том, что произошло "попадание". Это чаще всего рассматривается как режим аудита или бесшумного режима с помощью продуктов безопасности, в которых они просто регистрировали совпадение, но не выполняли действие. Значение по умолчанию − ложь.|
|severity|Int32|Набор, представляющий серьезность вредоносного поведения, определяемого данными в индикаторе. Допустимые значения : 0 — 5, где 5 является самым строгим, а нуль — не очень серьезным. Значение по умолчанию: 3.|
|tags|Коллекция String|Массив строк JSON, который хранит произвольные теги и ключевые слова.|
|tlpLevel|[tlpLevel](../resources/tiindicator.md#tlplevel-values)| Значение Протокола светофора для индикатора. Возможные значения: `unknown`, `white`, `green`, `amber`, `red`.|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется необязательный заголовок запроса, метод возвращает код ответа и обновленный `200 OK` [объект tiIndicator](../resources/tiindicator.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-request-without-prefer-header"></a>Пример 1. Запрос без загона Prefer

#### <a name="request"></a>Запрос

Ниже приводится пример запроса без `Prefer` загона.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-tiindicator-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-tiindicator-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Пример 2. Запрос с помощью загона Prefer

#### <a name="request"></a>Запрос

Ниже приводится пример запроса, включаемого `Prefer` в заглавную.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_2"
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-tiindicator-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-tiindicator-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> [!NOTE]
> Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.

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


