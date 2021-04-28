---
title: Обновление ipnamedlocation
description: Обновление свойств объекта ipNamedLocation.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6bd0c99094741b9d015ec5878afa819fe8794889
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051356"
---
# <a name="update-ipnamedlocation"></a><span data-ttu-id="cb87a-103">Обновление ipNamedlocation</span><span class="sxs-lookup"><span data-stu-id="cb87a-103">Update ipNamedlocation</span></span>

<span data-ttu-id="cb87a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb87a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb87a-105">Обновление свойств объекта [ipNamedLocation.](../resources/ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="cb87a-105">Update the properties of an [ipNamedLocation](../resources/ipNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb87a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb87a-106">Permissions</span></span>

<span data-ttu-id="cb87a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb87a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb87a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb87a-109">Permission type</span></span>                        | <span data-ttu-id="cb87a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb87a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb87a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb87a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb87a-112">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="cb87a-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="cb87a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb87a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb87a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb87a-114">Not supported.</span></span> |
| <span data-ttu-id="cb87a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb87a-115">Application</span></span>                            | <span data-ttu-id="cb87a-116">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="cb87a-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb87a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb87a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cb87a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb87a-118">Request headers</span></span>

| <span data-ttu-id="cb87a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cb87a-119">Name</span></span>       | <span data-ttu-id="cb87a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cb87a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cb87a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb87a-121">Authorization</span></span> | <span data-ttu-id="cb87a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb87a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb87a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb87a-124">Content-type</span></span> | <span data-ttu-id="cb87a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb87a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb87a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb87a-127">Request body</span></span>

<span data-ttu-id="cb87a-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="cb87a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cb87a-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="cb87a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cb87a-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="cb87a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cb87a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb87a-131">Property</span></span>     | <span data-ttu-id="cb87a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="cb87a-132">Type</span></span>        | <span data-ttu-id="cb87a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cb87a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb87a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cb87a-134">displayName</span></span>|<span data-ttu-id="cb87a-135">String</span><span class="sxs-lookup"><span data-stu-id="cb87a-135">String</span></span>|<span data-ttu-id="cb87a-136">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="cb87a-136">Human-readable name of the location.</span></span>|
|<span data-ttu-id="cb87a-137">ipRanges</span><span class="sxs-lookup"><span data-stu-id="cb87a-137">ipRanges</span></span>|<span data-ttu-id="cb87a-138">Коллекция объектов [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="cb87a-138">[ipRange](../resources/iprange.md) collection</span></span>|<span data-ttu-id="cb87a-139">Список диапазонов IP-адресов в формате CIDR IPv4 (1.2.3.4/32) или любого допустимого формата IPv6 от IETF RFC5962.</span><span class="sxs-lookup"><span data-stu-id="cb87a-139">List of IP address ranges in IPv4 CIDR format (1.2.3.4/32) or any allowable IPv6 format from IETF RFC5962.</span></span>|
|<span data-ttu-id="cb87a-140">isTrusted</span><span class="sxs-lookup"><span data-stu-id="cb87a-140">isTrusted</span></span>|<span data-ttu-id="cb87a-141">Логический</span><span class="sxs-lookup"><span data-stu-id="cb87a-141">Boolean</span></span>|<span data-ttu-id="cb87a-142">Значение, если `true` это расположение явно доверяется.</span><span class="sxs-lookup"><span data-stu-id="cb87a-142">The value is `true` if this location is explicitly trusted.</span></span>|

## <a name="response"></a><span data-ttu-id="cb87a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb87a-143">Response</span></span>

<span data-ttu-id="cb87a-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cb87a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb87a-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb87a-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb87a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb87a-147">Request</span></span>

<span data-ttu-id="cb87a-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb87a-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cb87a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb87a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
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
# <a name="c"></a>[<span data-ttu-id="cb87a-150">C#</span><span class="sxs-lookup"><span data-stu-id="cb87a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ipnamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb87a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb87a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ipnamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb87a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb87a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ipnamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb87a-153">Java</span><span class="sxs-lookup"><span data-stu-id="cb87a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ipnamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb87a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb87a-154">Response</span></span>

<span data-ttu-id="cb87a-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cb87a-155">The following is an example of the response.</span></span>

> <span data-ttu-id="cb87a-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cb87a-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
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

