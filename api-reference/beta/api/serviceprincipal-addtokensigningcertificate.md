---
title: 'servicePrincipal: addTokenSigningCertificate'
description: Добавьте сертификат подписи в службуPrincipal.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 01aded24ecce1b15c7bb56b9c5054f887098dc38
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787228"
---
# <a name="serviceprincipal-addtokensigningcertificate"></a><span data-ttu-id="08c8a-103">servicePrincipal: addTokenSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="08c8a-103">servicePrincipal: addTokenSigningCertificate</span></span>

<span data-ttu-id="08c8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08c8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08c8a-105">Создает самозаверяемый сертификат подписи и возвращает [selfSignedCertificate](../resources/selfsignedcertificate.md), который является публичной частью сгенерированного сертификата.</span><span class="sxs-lookup"><span data-stu-id="08c8a-105">Creates a self-signed signing certificate and returns a [selfSignedCertificate](../resources/selfsignedcertificate.md), which is the public part of the generated certificate.</span></span> <span data-ttu-id="08c8a-106">Самозаверяется сертификат подписи состоит из этих ресурсов: частный ключ[(keyCredential](../resources/keycredential.md) с использованием = "Sign"), общедоступный ключ[(keyCredential](../resources/keycredential.md) с использованием = "verify") и [passwordCredential](../resources/passwordcredential.md).</span><span class="sxs-lookup"><span data-stu-id="08c8a-106">The self-signed signing certificate is composed of these resources: the private key ([keyCredential](../resources/keycredential.md) with usage = 'Sign'), the public key ([keyCredential](../resources/keycredential.md) with usage = 'verify'), and the [passwordCredential](../resources/passwordcredential.md).</span></span> <span data-ttu-id="08c8a-107">Все созданные ресурсы имеют один и тот же **настраиваемыйKeyIdentifier.**</span><span class="sxs-lookup"><span data-stu-id="08c8a-107">All the created resources have the same **customKeyIdentifier**.</span></span>

<span data-ttu-id="08c8a-108">**ПарольCredential используется** для открытия ключа pfx/private.</span><span class="sxs-lookup"><span data-stu-id="08c8a-108">The **passwordCredential** is used to open the pfx/private key.</span></span> <span data-ttu-id="08c8a-109">Кроме того, это связано с privateKey с тем же **keyId**.</span><span class="sxs-lookup"><span data-stu-id="08c8a-109">Also, it's associated with the privateKey having the same **keyId**.</span></span> <span data-ttu-id="08c8a-110">Предмет сертификата — это постоянное значение.</span><span class="sxs-lookup"><span data-stu-id="08c8a-110">The subject of the certificate is a constant value.</span></span> <span data-ttu-id="08c8a-111">На нее не влияет необязательный **displayName,** предоставляемый в вызове POST.</span><span class="sxs-lookup"><span data-stu-id="08c8a-111">It won't be affected by the optional **displayName** provided in the POST call.</span></span> <span data-ttu-id="08c8a-112">**StartDateTime** задан в то же время, когда сертификат создается с помощью действия.</span><span class="sxs-lookup"><span data-stu-id="08c8a-112">The **startDateTime** is set to the same time the certificate is created using the action.</span></span> <span data-ttu-id="08c8a-113">**EndDateTime** может быть до трех лет после создания сертификата.</span><span class="sxs-lookup"><span data-stu-id="08c8a-113">The **endDateTime** can be up to three years after the certificate is created.</span></span>

## <a name="permissions"></a><span data-ttu-id="08c8a-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08c8a-114">Permissions</span></span>

|<span data-ttu-id="08c8a-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08c8a-115">Permission type</span></span>      | <span data-ttu-id="08c8a-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08c8a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08c8a-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08c8a-117">Delegated (work or school account)</span></span> | <span data-ttu-id="08c8a-118">Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08c8a-118">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="08c8a-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08c8a-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08c8a-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="08c8a-120">None.</span></span>    |
|<span data-ttu-id="08c8a-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="08c8a-121">Application</span></span> | <span data-ttu-id="08c8a-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08c8a-122">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="08c8a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08c8a-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addTokenSigningCertificate
```

## <a name="request-body"></a><span data-ttu-id="08c8a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08c8a-124">Request body</span></span>

<span data-ttu-id="08c8a-125">В теле запроса укажи следующие необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="08c8a-125">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="08c8a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="08c8a-126">Property</span></span>     | <span data-ttu-id="08c8a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="08c8a-127">Type</span></span>   |<span data-ttu-id="08c8a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="08c8a-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08c8a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="08c8a-129">displayName</span></span> | <span data-ttu-id="08c8a-130">string</span><span class="sxs-lookup"><span data-stu-id="08c8a-130">string</span></span> | <span data-ttu-id="08c8a-131">Удобное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="08c8a-131">Friendly name for the key.</span></span>  <span data-ttu-id="08c8a-132">Она должна начинаться `CN=` с .</span><span class="sxs-lookup"><span data-stu-id="08c8a-132">It must start with `CN=`.</span></span>|
| <span data-ttu-id="08c8a-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="08c8a-133">endDateTime</span></span> | <span data-ttu-id="08c8a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08c8a-134">DateTimeOffset</span></span> |<span data-ttu-id="08c8a-135">Дата и время истечения срока действия учетных данных.</span><span class="sxs-lookup"><span data-stu-id="08c8a-135">The date and time when the credential expires.</span></span> <span data-ttu-id="08c8a-136">Срок создания сертификата может быть не более 3 лет.</span><span class="sxs-lookup"><span data-stu-id="08c8a-136">It can be up to 3 years from the date the certificate is created.</span></span> <span data-ttu-id="08c8a-137">Если она не предоставлена, по умолчанию — три года со времени создания.</span><span class="sxs-lookup"><span data-stu-id="08c8a-137">If not supplied, the default is three years from the time of creation.</span></span> <span data-ttu-id="08c8a-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="08c8a-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08c8a-139">Например, полночь UTC 1 января 2014 г. будет выглядеть так: '2014-01-01T00:00:00Z' .</span><span class="sxs-lookup"><span data-stu-id="08c8a-139">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z' .</span></span>|

## <a name="response"></a><span data-ttu-id="08c8a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="08c8a-140">Response</span></span>

<span data-ttu-id="08c8a-141">В случае успеха этот метод возвращает код ответа и `200 OK` новый [объект selfSignedCertificate](../resources/selfsignedcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="08c8a-141">If successful, this method returns a `200 OK` response code and a new [selfSignedCertificate](../resources/selfsignedcertificate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08c8a-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="08c8a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08c8a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="08c8a-143">Request</span></span>

<span data-ttu-id="08c8a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08c8a-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08c8a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="08c8a-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="08c8a-146">C#</span><span class="sxs-lookup"><span data-stu-id="08c8a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addtokensigningcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08c8a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08c8a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addtokensigningcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08c8a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08c8a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addtokensigningcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08c8a-149">Java</span><span class="sxs-lookup"><span data-stu-id="08c8a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addtokensigningcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08c8a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="08c8a-150">Response</span></span>

<span data-ttu-id="08c8a-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08c8a-151">The following is an example of the response.</span></span>

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

