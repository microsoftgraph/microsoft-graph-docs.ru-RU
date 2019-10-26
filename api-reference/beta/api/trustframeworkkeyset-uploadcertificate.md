---
title: 'Трустфрамеворккэйсет: Уплоадцертификате'
description: Отправьте сертификат в набор ключей.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64e5354cb39f2c2ead70b32f46f06c64615dfca2
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734688"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="26adc-103">Трустфрамеворккэйсет: Уплоадцертификате</span><span class="sxs-lookup"><span data-stu-id="26adc-103">trustFrameworkKeySet: uploadCertificate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26adc-104">Отправьте сертификат в [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="26adc-104">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="26adc-105">Входное значение — это значение сертификата в кодировке Base-64.</span><span class="sxs-lookup"><span data-stu-id="26adc-105">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="26adc-106">Этот метод возвращает [трустфрамеворккэй](../resources/trustframeworkkey.md).</span><span class="sxs-lookup"><span data-stu-id="26adc-106">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="26adc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26adc-107">Permissions</span></span>

<span data-ttu-id="26adc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26adc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26adc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26adc-110">Permission type</span></span>                        | <span data-ttu-id="26adc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26adc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26adc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26adc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="26adc-113">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="26adc-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="26adc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26adc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26adc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26adc-115">Not supported.</span></span> |
| <span data-ttu-id="26adc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26adc-116">Application</span></span>                            | <span data-ttu-id="26adc-117">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="26adc-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26adc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26adc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="26adc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26adc-119">Request headers</span></span>

| <span data-ttu-id="26adc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="26adc-120">Name</span></span>          | <span data-ttu-id="26adc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="26adc-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26adc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26adc-122">Authorization</span></span> | <span data-ttu-id="26adc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26adc-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="26adc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26adc-125">Content-type</span></span> | <span data-ttu-id="26adc-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26adc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26adc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26adc-128">Request body</span></span>

<span data-ttu-id="26adc-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="26adc-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="26adc-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="26adc-130">Parameter</span></span>    | <span data-ttu-id="26adc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="26adc-131">Type</span></span>        | <span data-ttu-id="26adc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="26adc-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26adc-133">key</span><span class="sxs-lookup"><span data-stu-id="26adc-133">key</span></span>|<span data-ttu-id="26adc-134">String</span><span class="sxs-lookup"><span data-stu-id="26adc-134">String</span></span>| <span data-ttu-id="26adc-135">Это поле для отправки контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="26adc-135">This is the field for sending certificate content.</span></span> <span data-ttu-id="26adc-136">Значение должно представлять собой версию фактического содержимого сертификата в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="26adc-136">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="26adc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="26adc-137">Response</span></span>

<span data-ttu-id="26adc-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [трустфрамеворккэй](../resources/trustframeworkkey.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26adc-138">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26adc-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="26adc-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26adc-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="26adc-140">Request</span></span>

<span data-ttu-id="26adc-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26adc-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadCertificate
Content-type: application/json

{
  "key": "key-value"
}
```

### <a name="response"></a><span data-ttu-id="26adc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="26adc-142">Response</span></span>

<span data-ttu-id="26adc-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26adc-143">The following is an example of the response.</span></span>

> <span data-ttu-id="26adc-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26adc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "sig",
    "kty": "oct",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
