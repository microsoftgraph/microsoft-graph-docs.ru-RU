---
title: 'servicePrincipal: addTokenSigningCertificate'
description: Добавьте сертификат подписи в службуPrincipal.
ms.localizationpriority: medium
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0b835c493916f1f6216ba87625670538db96904b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026325"
---
# <a name="serviceprincipal-addtokensigningcertificate"></a>servicePrincipal: addTokenSigningCertificate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает самозаверяемый сертификат подписи и возвращает объект [selfSignedCertificate,](../resources/selfsignedcertificate.md) который является публичной частью сгенерированного сертификата. Самозаверяется сертификат подписи состоит из следующих объектов, которые добавляются в [службуPrincipal:](../resources/serviceprincipal.md) 
+ Объект [keyCredentials со](../resources/keycredential.md) следующими объектами:
    + Частный объект ключа **с набором** использования `Sign` .
    + Объект public key с **набором** использования `Verify` .
+ Объект [passwordCredentials.](../resources/passwordcredential.md)

Все объекты имеют одинаковое значение **customKeyIdentifier**.

**ПарольCredential используется** для открытия файла PFX (закрытый ключ). Он и связанный частный объект ключа имеют одинаковое значение **keyId**. После набора во время создания с помощью **свойства displayName** объект сертификата не может быть обновлен. **StartDateTime** задан в то же время, когда сертификат создается с помощью действия. **EndDateTime** может быть до трех лет после создания сертификата.

## <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All, Directory.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Нет.    |
|Приложение | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |


## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addTokenSigningCertificate
```

## <a name="request-body"></a>Текст запроса

В теле запроса укажи следующие необходимые свойства.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| displayName | string | Удобное имя для ключа.  Она должна начинаться `CN=` с .|
| endDateTime | DateTimeOffset |Дата и время истечения срока действия учетных данных. Срок создания сертификата может быть не более 3 лет. Если она не предоставлена, по умолчанию — три года со времени создания. Тип timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа и `200 OK` новый [объект selfSignedCertificate](../resources/selfsignedcertificate.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addtokensigningcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/004375c5-6e2e-4dec-95e3-626838cb9f80/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=customDisplayName",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addtokensigningcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addtokensigningcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addtokensigningcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addtokensigningcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-addtokensigningcertificate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.selfSignedCertificate"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "2iD8ppbE+D6Kmu1ZvjM2jtQh88E=",
  "displayName": "CN=customDisplayName",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICuDCCAaCgAwIBAgIIYXJsNtL4oUMwDQYJKoZIhvcNAQEL...StP8s/w==",
  "keyId": "93bc223f-7235-4b9c-beea-d66847531c49",
  "startDateTime": "2021-05-05T18:38:51.8100763Z",
  "thumbprint": "DA20FCA696C4F83E8A9AED59BE33368ED421F3C1",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-01-15 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: selfSignedCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
} -->

