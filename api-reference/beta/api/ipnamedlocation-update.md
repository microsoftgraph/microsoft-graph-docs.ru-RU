---
title: Обновление ipnamedlocation
description: Обновление свойств объекта ipNamedLocation.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3afd3800d462936686197fb86e1b1e458ab7997c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786925"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="26204-103">Обновление ipNamedlocation</span><span class="sxs-lookup"><span data-stu-id="26204-103">Update ipNamedlocation</span></span>

<span data-ttu-id="26204-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26204-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26204-105">Обновление свойств объекта [ipNamedLocation.](../resources/ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="26204-105">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26204-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26204-106">Permissions</span></span>

<span data-ttu-id="26204-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26204-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26204-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26204-109">Permission type</span></span>                        | <span data-ttu-id="26204-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26204-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26204-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26204-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26204-112">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="26204-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="26204-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26204-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26204-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26204-114">Not supported.</span></span> |
| <span data-ttu-id="26204-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="26204-115">Application</span></span>                            | <span data-ttu-id="26204-116">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="26204-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="26204-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26204-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="26204-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26204-118">Request headers</span></span>

| <span data-ttu-id="26204-119">Имя</span><span class="sxs-lookup"><span data-stu-id="26204-119">Name</span></span>       | <span data-ttu-id="26204-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26204-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="26204-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26204-121">Authorization</span></span> | <span data-ttu-id="26204-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26204-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26204-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26204-124">Content-type</span></span> | <span data-ttu-id="26204-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26204-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26204-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26204-127">Request body</span></span>

<span data-ttu-id="26204-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="26204-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="26204-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="26204-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="26204-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="26204-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26204-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="26204-131">Property</span></span>     | <span data-ttu-id="26204-132">Тип</span><span class="sxs-lookup"><span data-stu-id="26204-132">Type</span></span>        | <span data-ttu-id="26204-133">Описание</span><span class="sxs-lookup"><span data-stu-id="26204-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26204-134">displayName</span><span class="sxs-lookup"><span data-stu-id="26204-134">displayName</span></span>|<span data-ttu-id="26204-135">String</span><span class="sxs-lookup"><span data-stu-id="26204-135">String</span></span>|<span data-ttu-id="26204-136">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="26204-136">Human-readable name of the location.</span></span>|
|<span data-ttu-id="26204-137">ipRanges</span><span class="sxs-lookup"><span data-stu-id="26204-137">ipRanges</span></span>|<span data-ttu-id="26204-138">Коллекция объектов [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="26204-138">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="26204-139">Список диапазонов IP-адресов в формате CIDR IPv4 (1.2.3.4/32) или любого допустимого формата IPv6 от IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="26204-139">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="26204-140">isTrusted</span><span class="sxs-lookup"><span data-stu-id="26204-140">isTrusted</span></span>|<span data-ttu-id="26204-141">Логический</span><span class="sxs-lookup"><span data-stu-id="26204-141">Boolean</span></span>|<span data-ttu-id="26204-142">Значение, если `true` это расположение явно доверяется.</span><span class="sxs-lookup"><span data-stu-id="26204-142">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="26204-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="26204-143">Response</span></span>

<span data-ttu-id="26204-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26204-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26204-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="26204-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26204-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="26204-147">Request</span></span>

<span data-ttu-id="26204-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26204-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26204-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="26204-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.ipNamedLocation",
    "displayName": "Untrusted named location with only IPv4 address",
    "isTrusted": false,
    "ipRanges": [
        {
            "@odata.type": "#microsoft.graph.iPv4CidrRange",
            "cidrAddress": "6.5.4.3/18"
        }

    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="26204-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26204-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="26204-151">C#</span><span class="sxs-lookup"><span data-stu-id="26204-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26204-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26204-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26204-153">Java</span><span class="sxs-lookup"><span data-stu-id="26204-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ipnamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26204-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="26204-154">Response</span></span>

<span data-ttu-id="26204-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="26204-155">The following is an example of the response.</span></span>

> <span data-ttu-id="26204-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26204-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update ipnamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


