---
title: Обновление объектов secureScoreControlProfile
description: Обновление редактируемого объекта Секурескореконтролпрофиле в любом интегрированном решении для изменения различных свойств, таких как assignedTo или Тенантноте.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6192d33e2d7d1b98e61a4d9f28f863cd03e234d7
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330370"
---
# <a name="update-securescorecontrolprofile"></a>Обновление объектов secureScoreControlProfile

Пространство имен: microsoft.graph

Обновление редактируемого объекта **секурескореконтролпрофиле** в любом интегрированном решении для изменения различных свойств, таких как **assignedTo** или **тенантноте**.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |   SecurityEvents.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Приложение | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {код}. Обязательно.|
|Prefer | Возврат = представление. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление значений в формате JSON для соответствующих полей, которые необходимо обновить. Текст **должен** содержать `vendorInformation` Свойство Valid `provider` и `vendor` Fields. В следующей таблице перечислены поля, которые можно обновить для **секурескореконтролпрофиле**. Значения для существующих свойств, не включенных в текст запроса, не изменятся. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|assignedTo|String|Имя аналитики, которой назначен элемент управления для рассмотрения, внедрения или исправления.|
|comment|String|Комментарии аналитика в элементе управления (для управления клиентом).|
|state| String|Управляемый аналитикой параметр для элемента управления. Возможные значения: `Default`, `Ignored`, `ThirdParty`, `Reviewed`.|
| vendorInformation | [securityVendorInformation](../resources/securityvendorinformation.md) | Сложный тип, содержащий сведения о продукте, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре;). **Требуются поля поставщика и поставщика.** |


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется заголовок необязательного запроса, метод возвращает `200 OK` код отклика и обновленный объект [секурескореконтролпрофилес](../resources/securescorecontrolprofile.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="example-1-request-without-prefer-header"></a>Пример 1: запрос без верхнего колонтитула

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {

    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже представлен пример успешного отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Пример 2: запрос с заголовком предпочтения

#### <a name="request"></a>Запрос

В приведенном ниже примере показан запрос, включающий `Prefer` заголовок запроса.

<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/NonOwnerAccess
Content-type: application/json

{
  "assignedTo": "",
  "comment": "control is reviewed",
  "state": "Reviewed",
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика при использовании заголовка необязательного `Prefer: return=representation` запроса.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "NonOwnerAccess",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Review",
  "actionUrl": "https://outlook.office365.com/NonOwnerAccessReport.aspx",
  "controlCategory": "Data",
  "title": "Review mailbox access by non-owners bi-weekly", 
  "deprecated": false,
  "implementationCost": "Low",
  "lastModifiedDateTime": null,
  "maxScore": 5.0,
  "rank": 25,
  "remediation": "Once you have opened the search tool, specify a date range and select access by <b>All non-owners</b> or <b>External users</b>",
  "remediationImpact": "This change will have no effect on your users",
  "service": "EXO",
  "threats": [
    "Account Breach",
    "Data Exfiltration",
    "Malicious Insider"
  ],
  "tier": "Core",
  "userImpact": "Low",
  "complianceInformation": [
    {
      "certificationName": "FedRAMP_Moderate",
      "certificationControls": [
        {
          "name": "AC-6(9)",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": "",
      "comment": "control is reviewed",
      "state": "Reviewed",
      "updatedBy": "user1@contoso.com",
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
    }
  ],
  "vendorInformation": {
    "provider": "SecureScore",
    "providerVersion": null,
    "subProvider": null,
    "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

