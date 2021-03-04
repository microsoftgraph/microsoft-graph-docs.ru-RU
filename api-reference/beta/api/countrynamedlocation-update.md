---
title: Обновление countryNamedlocation
description: Обновление свойств объекта countryNamedLocation.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5827219409f49e5e27eed9539c23609cf126bf02
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437249"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="8bb13-103">Обновление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="8bb13-103">Update countryNamedLocation</span></span>

<span data-ttu-id="8bb13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bb13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb13-105">Обновление свойств объекта [countryNamedLocation.](../resources/countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="8bb13-105">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb13-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb13-106">Permissions</span></span>

<span data-ttu-id="8bb13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bb13-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb13-109">Permission type</span></span>                        | <span data-ttu-id="8bb13-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bb13-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8bb13-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bb13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bb13-112">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="8bb13-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="8bb13-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bb13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb13-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb13-114">Not supported.</span></span> |
| <span data-ttu-id="8bb13-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8bb13-115">Application</span></span>                            | <span data-ttu-id="8bb13-116">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="8bb13-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bb13-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bb13-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bb13-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bb13-118">Request headers</span></span>

| <span data-ttu-id="8bb13-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8bb13-119">Name</span></span>       | <span data-ttu-id="8bb13-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb13-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8bb13-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bb13-121">Authorization</span></span> | <span data-ttu-id="8bb13-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bb13-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8bb13-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bb13-124">Content-type</span></span>  | <span data-ttu-id="8bb13-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bb13-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bb13-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bb13-127">Request body</span></span>

<span data-ttu-id="8bb13-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8bb13-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8bb13-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8bb13-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8bb13-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8bb13-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8bb13-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bb13-131">Property</span></span>     | <span data-ttu-id="8bb13-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb13-132">Type</span></span>        | <span data-ttu-id="8bb13-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb13-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8bb13-134">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="8bb13-134">countriesAndRegions</span></span>|<span data-ttu-id="8bb13-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8bb13-135">String collection</span></span>|<span data-ttu-id="8bb13-136">Список стран и/или регионов в формате двух букв, заданный ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="8bb13-136">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="8bb13-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8bb13-137">displayName</span></span>|<span data-ttu-id="8bb13-138">String</span><span class="sxs-lookup"><span data-stu-id="8bb13-138">String</span></span>|<span data-ttu-id="8bb13-139">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="8bb13-139">Human-readable name of the location.</span></span>|
|<span data-ttu-id="8bb13-140">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="8bb13-140">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="8bb13-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bb13-141">Boolean</span></span>|<span data-ttu-id="8bb13-142">Значение в том случае, если IP-адреса, которые не относятся к стране или региону, должны быть включены `true` в именоваемом расположении.</span><span class="sxs-lookup"><span data-stu-id="8bb13-142">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="8bb13-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb13-143">Response</span></span>

<span data-ttu-id="8bb13-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8bb13-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bb13-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="8bb13-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bb13-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bb13-147">Request</span></span>

<span data-ttu-id="8bb13-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bb13-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bb13-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb13-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Updated named location without unknown countries and regions",
    "countriesAndRegions": [
        "CA",
        "IN"
    ],
    "includeUnknownCountriesAndRegions": false
}
```
# <a name="javascript"></a>[<span data-ttu-id="8bb13-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb13-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bb13-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bb13-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8bb13-152">C#</span><span class="sxs-lookup"><span data-stu-id="8bb13-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bb13-153">Java</span><span class="sxs-lookup"><span data-stu-id="8bb13-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8bb13-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb13-154">Response</span></span>

<span data-ttu-id="8bb13-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8bb13-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update countrynamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


