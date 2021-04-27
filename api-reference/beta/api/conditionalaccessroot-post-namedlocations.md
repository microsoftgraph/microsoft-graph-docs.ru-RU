---
title: Создание namedLocation
description: Создайте новое имяLocation.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 51b661169dc1e308f3e7e422b1ba8eec4843de56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047233"
---
# <a name="create-namedlocation"></a><span data-ttu-id="29808-103">Создание namedLocation</span><span class="sxs-lookup"><span data-stu-id="29808-103">Create namedLocation</span></span>

<span data-ttu-id="29808-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29808-105">Создайте новый [объект с именемLocation.](../resources/namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="29808-105">Create a new [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="29808-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29808-106">Permissions</span></span>

<span data-ttu-id="29808-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29808-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29808-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29808-109">Permission type</span></span>                        | <span data-ttu-id="29808-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29808-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29808-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29808-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29808-112">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="29808-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="29808-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29808-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29808-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29808-114">Not supported.</span></span> |
| <span data-ttu-id="29808-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29808-115">Application</span></span>                            | <span data-ttu-id="29808-116">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="29808-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="29808-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29808-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/namedLocations
```

## <a name="request-headers"></a><span data-ttu-id="29808-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29808-118">Request headers</span></span>

| <span data-ttu-id="29808-119">Имя</span><span class="sxs-lookup"><span data-stu-id="29808-119">Name</span></span>          | <span data-ttu-id="29808-120">Описание</span><span class="sxs-lookup"><span data-stu-id="29808-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="29808-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29808-121">Authorization</span></span> | <span data-ttu-id="29808-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29808-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29808-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29808-124">Content-Type</span></span>  | <span data-ttu-id="29808-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29808-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29808-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29808-127">Request body</span></span>

<span data-ttu-id="29808-128">В теле запроса укажи представление JSON объекта [ipNamedLocation](../resources/ipnamedlocation.md) или [countryNamedLocation.](../resources/countrynamedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="29808-128">In the request body, supply a JSON representation of an [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="29808-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="29808-129">Response</span></span>

<span data-ttu-id="29808-130">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект ipNamedLocation](../resources/ipnamedlocation.md) или [объект countryNamedLocation](../resources/countrynamedlocation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="29808-130">If successful, this method returns a `201 Created`response code and a new [ipNamedLocation](../resources/ipnamedlocation.md) or [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29808-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="29808-131">Examples</span></span>

### <a name="example-1-create-an-ipnamedlocation"></a><span data-ttu-id="29808-132">Пример 1. Создание ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="29808-132">Example 1: Create an ipNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="29808-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="29808-133">Request</span></span>

<span data-ttu-id="29808-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29808-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29808-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="29808-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot_1"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "displayName": "Untrusted IP named location",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="29808-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29808-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-namedlocation-from-conditionalaccessroot-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29808-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29808-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-namedlocation-from-conditionalaccessroot-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="29808-138">C#</span><span class="sxs-lookup"><span data-stu-id="29808-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-namedlocation-from-conditionalaccessroot-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29808-139">Java</span><span class="sxs-lookup"><span data-stu-id="29808-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-namedlocation-from-conditionalaccessroot-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29808-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="29808-140">Response</span></span>

<span data-ttu-id="29808-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="29808-141">The following is an example of the response.</span></span>

> <span data-ttu-id="29808-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="29808-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "id": "0854951d-5fc0-4eb1-b392-9b2c9d7949c2",
    "displayName": "Untrusted IP named location",
    "modifiedDateTime": "2019-09-04T01:11:34.9387578Z",
    "createdDateTime": "2019-09-04T01:11:34.9387578Z",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "12.34.221.11/22"
        },
        {
            "@odata.type": "#microsoft.graph.iPv6CidrRange",
            "cidrAddress": "2001:0:9d38:90d6:0:0:0:0/63"
        }
    ]
}
```
### <a name="example-2-create-a-countrynamedlocation"></a><span data-ttu-id="29808-143">Пример 2. Создание страныNamedLocation</span><span class="sxs-lookup"><span data-stu-id="29808-143">Example 2: Create a countryNamedLocation</span></span>

#### <a name="request"></a><span data-ttu-id="29808-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="29808-144">Request</span></span>

<span data-ttu-id="29808-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29808-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29808-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="29808-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_namedlocation_from_conditionalaccessroot_2"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Named location with unknown countries and regions",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```
# <a name="c"></a>[<span data-ttu-id="29808-147">C#</span><span class="sxs-lookup"><span data-stu-id="29808-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-namedlocation-from-conditionalaccessroot-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29808-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29808-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-namedlocation-from-conditionalaccessroot-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29808-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29808-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-namedlocation-from-conditionalaccessroot-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29808-150">Java</span><span class="sxs-lookup"><span data-stu-id="29808-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-namedlocation-from-conditionalaccessroot-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29808-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="29808-151">Response</span></span>

<span data-ttu-id="29808-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="29808-152">The following is an example of the response.</span></span>

> <span data-ttu-id="29808-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="29808-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#namedLocations/$entity",
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "id": "1c4427fd-0885-4a3d-8b23-09a899ffa959",
    "displayName": "Named location with unknown countries and regions",
    "modifiedDateTime": "2019-09-04T01:08:02.5249255Z",
    "createdDateTime": "2019-09-04T01:08:02.5249255Z",
    "countriesAndRegions": [
        "US",
        "GB"
    ],
    "includeUnknownCountriesAndRegions": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


