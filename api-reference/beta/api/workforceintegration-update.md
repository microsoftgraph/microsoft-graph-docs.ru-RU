---
title: Обновление воркфорцеинтегратион
description: Обновление свойств объекта воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 80b688d700dff94d1a746e651b83a4b0236d1a39
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44154404"
---
# <a name="update-workforceintegration"></a>Обновление воркфорцеинтегратион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     |Воркфорцеинтегратион. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Authorization | Bearer {token} |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|апиверсион|Int32|Версия API для URL-адреса обратного вызова. Начните с 1.|
|displayName|String|Имя интеграции трудовых ресурсов.|
|шифрования|воркфорцеинтегратионенкриптион|Ресурс для шифрования взаимодействия сотрудников. |
|isActive|Boolean|Указывает, активна ли эта интеграция сотрудников в настоящее время и доступна ли она.|
|имеется|string| Возможные значения:,,,, `none` `shift` `swapRequest` `openshift` `openShiftRequest` , `userShiftPreferences` . Если выбрано более одного значения, все значения должны начинаться с первой буквы в верхнем регистре.|
|суппортедентитиес|string| Это свойство **будет заменено** в версии 1.0. Мы рекомендуем использовать это свойство вместо **поддерживаемых**. Свойство **Supports будет по-** прежнему поддерживаться в бета-версии в течение этого времени. Возможные значения:,,,, `none` `shift` `swapRequest` `openshift` `openShiftRequest` , `userShiftPreferences` . Если выбрано более одного значения, все значения должны начинаться с первой буквы в верхнем регистре.|
|url|String| URL-адрес интеграции сотрудников для обратных вызовов из службы смены. |

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-update-a-workforceintegration-object"></a>Пример 1: обновление объекта Воркфорцеинтегратион

В приведенном ниже примере показано, как обновить объект **воркфорцеинтегратион** .

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a>Пример 2: создание нового Воркфорцеинтегратион с включенной функцией Свапрекуест для фильтрации допустимости

В следующем примере показано, как создать **воркфорцеинтегратион** с свапрекуест, включенным для фильтрации приемлемости.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. 
```
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations/
Authorization: Bearer {token}
Content-type: application/json

{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://ABCWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
#### <a name="response"></a>Ответ

Ниже приведен пример отклика.
```
HTTP/1.1 200 OK
{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
Чтобы создать новый **воркфорцеинтегратион** с включенной функцией фильтрации соответствия свапрекуест, ознакомьтесь со статьей метод [CREATE](../api/workforceintegration-post.md) .

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a>Пример 3: получение подходящих смен при включении Свапрекуест в Елигибилитифилтеринженабледентитиес

Конечные точки интеграции "взаимодействие между сменами приложения" и "ресурсы" будут соответствовать существующему шаблону.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса, сделанного сменам конечной точки интеграции сотрудников для получения подходящих смен для запроса на замену.

```
POST https://abcWorkforceIntegration.com/Contoso/{apiVersion}/team/{teamId}/read
Accept-Language: en-us

{
  "requests": [
  {
     "id": "{shiftId}",
     "method": "GET”,
     "url": “/shifts/{shiftId}/requestableShifts?requestType={requestType}&startDateTime={startDateTime}&endDateTime={endDateTime}”
   }]
}
```
#### <a name="response"></a>Ответ

Ниже приведен пример ответа от службы интеграции сотрудников.
```
HTTP/1.1 200 OK
{
  "responses": [
  {
    "body": {
      "SHFT_6548f642-cbc1-4228-8621-054327576457",
      "SHFT_6548f642-cbc1-4228-8621-054327571234"
  }
    "id": "{shiftId}",
    "status: 200,
    "body": {
       "data": [{ShiftId}, {ShiftId}...]
       "error": null
    }
  ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
