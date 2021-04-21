---
title: Get teamsAppIcon
description: Извлечение значка, связанного с определенным определением приложения Teams.
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7e80b20f0802fbfa084c02b9103e7362be9ca159
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921779"
---
# <a name="get-teamsappicon"></a><span data-ttu-id="47995-103">Get teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="47995-103">Get teamsAppIcon</span></span>

<span data-ttu-id="47995-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47995-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47995-105">[Извлечение значка приложения Teams,](../resources/teamsappicon.md) связанного с определенным [определением](../resources/teamsappdefinition.md) [приложения.](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="47995-105">Retrieve a [Teams app icon](../resources/teamsappicon.md) associated with a specific [definition](../resources/teamsappdefinition.md) of an [app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="47995-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47995-106">Permissions</span></span>

<span data-ttu-id="47995-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47995-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47995-109">Permission Type</span></span>                        | <span data-ttu-id="47995-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47995-110">Permissions (from least to most privileged)</span></span>                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="47995-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47995-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="47995-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="47995-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
| <span data-ttu-id="47995-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47995-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47995-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47995-114">Not supported.</span></span>                                                   |
| <span data-ttu-id="47995-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47995-115">Application</span></span>                            | <span data-ttu-id="47995-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47995-116">Not supported.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="47995-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47995-117">HTTP request</span></span>

<span data-ttu-id="47995-118">**Получить значок цвета определения приложения Teams**</span><span class="sxs-lookup"><span data-stu-id="47995-118">**Get color icon of a Teams app definition**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon
```

<span data-ttu-id="47995-119">**Получить значок контура определения приложения Teams**</span><span class="sxs-lookup"><span data-stu-id="47995-119">**Get outline icon of a Teams app definition**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47995-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47995-120">Optional query parameters</span></span>

<span data-ttu-id="47995-121">Эта операция поддерживает параметры `$select` `$expand` [запроса oData и OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47995-121">This operation supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47995-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47995-122">Request headers</span></span>

| <span data-ttu-id="47995-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47995-123">Header</span></span>           | <span data-ttu-id="47995-124">Значение</span><span class="sxs-lookup"><span data-stu-id="47995-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="47995-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47995-125">Authorization</span></span>    | <span data-ttu-id="47995-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47995-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47995-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47995-128">Request body</span></span>

<span data-ttu-id="47995-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47995-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47995-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="47995-130">Response</span></span>

<span data-ttu-id="47995-131">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [teamsAppIcon](../resources/teamsappicon.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="47995-131">If successful, this method returns a `200 OK` response code and a [teamsAppIcon](../resources/teamsappicon.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47995-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="47995-132">Examples</span></span>

### <a name="example-1-get-color-icon-of-a-custom-teams-app"></a><span data-ttu-id="47995-133">Пример 1. Получить значок цвета *настраиваемого* приложения Teams</span><span class="sxs-lookup"><span data-stu-id="47995-133">Example 1: Get color icon of a *custom* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="47995-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="47995-134">Request</span></span>

<span data-ttu-id="47995-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47995-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47995-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="47995-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_coloricon_customapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon
```
# <a name="c"></a>[<span data-ttu-id="47995-137">C#</span><span class="sxs-lookup"><span data-stu-id="47995-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamsappicon-coloricon-customapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47995-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47995-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamsappicon-coloricon-customapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47995-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47995-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamsappicon-coloricon-customapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47995-140">Java</span><span class="sxs-lookup"><span data-stu-id="47995-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamsappicon-coloricon-customapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="47995-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="47995-141">Response</span></span>

<span data-ttu-id="47995-142">В следующем примере показан ответ для организационного приложения.</span><span class="sxs-lookup"><span data-stu-id="47995-142">The following example shows the response for an organizational app.</span></span> 
> <span data-ttu-id="47995-143">**Примечание.** Для доступа к [фактическому](teamworkhostedcontent-get.md) изображению значка настраиваемого приложения требуется задать маркер Microsoft Graph в запросе.</span><span class="sxs-lookup"><span data-stu-id="47995-143">**Note**: Accessing the actual [image of the custom app's icon](teamworkhostedcontent-get.md) requires a Microsoft Graph token to be set on the request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/$entity",
    "id": "aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "webUrl": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/$value"
}
```

### <a name="example-2-get-outline-icon-of-a-custom-teams-app"></a><span data-ttu-id="47995-144">Пример 2. Получить значок контура *настраиваемого* приложения Teams</span><span class="sxs-lookup"><span data-stu-id="47995-144">Example 2: Get outline icon of a *custom* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="47995-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="47995-145">Request</span></span>

<span data-ttu-id="47995-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47995-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47995-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="47995-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_customapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon
```
# <a name="c"></a>[<span data-ttu-id="47995-148">C#</span><span class="sxs-lookup"><span data-stu-id="47995-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamsappicon-outlineicon-customapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47995-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47995-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamsappicon-outlineicon-customapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47995-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47995-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamsappicon-outlineicon-customapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47995-151">Java</span><span class="sxs-lookup"><span data-stu-id="47995-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamsappicon-outlineicon-customapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="47995-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="47995-152">Response</span></span>

<span data-ttu-id="47995-153">В следующем примере показан ответ для организационного приложения.</span><span class="sxs-lookup"><span data-stu-id="47995-153">The following example shows the response for an organizational app.</span></span> 
> <span data-ttu-id="47995-154">**Примечание.** Для доступа к [фактическому](teamworkhostedcontent-get.md) изображению значка настраиваемого приложения требуется задать маркер Microsoft Graph в запросе.</span><span class="sxs-lookup"><span data-stu-id="47995-154">**Note**:  Accessing the actual [image of the custom app's icon](teamworkhostedcontent-get.md) requires a Microsoft Graph token to be set on the request.</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/outlineIcon/$entity",
    "id": "aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWIxYzU0Mzg0NGE5ZmFjY2Y2YWI4NDdkNWY0NTU0ZGU0L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "webUrl": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value"
}
```


### <a name="example-3-get-color-icon-of-a-store-teams-app"></a><span data-ttu-id="47995-155">Пример 3. Получить значок цвета приложения *Store* Teams</span><span class="sxs-lookup"><span data-stu-id="47995-155">Example 3: Get color icon of a *store* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="47995-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="47995-156">Request</span></span>

<span data-ttu-id="47995-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47995-157">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47995-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="47995-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_publicapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/colorIcon/
```
# <a name="c"></a>[<span data-ttu-id="47995-159">C#</span><span class="sxs-lookup"><span data-stu-id="47995-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamsappicon-outlineicon-publicapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47995-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47995-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamsappicon-outlineicon-publicapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47995-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47995-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamsappicon-outlineicon-publicapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47995-162">Java</span><span class="sxs-lookup"><span data-stu-id="47995-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamsappicon-outlineicon-publicapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="47995-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="47995-163">Response</span></span>

<span data-ttu-id="47995-164">В следующем примере показан ответ для приложения магазина.</span><span class="sxs-lookup"><span data-stu-id="47995-164">The following example shows the response for a store app.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://canary.graph.microsoft.com/testprodbetateamsgraphdev/$metadata#appCatalogs/teamsApps('95de633a-083e-42f5-b444-a4295d8e9314')/appDefinitions('OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk')/colorIcon/$entity",
    "id": "aHR0cHM6Ly9zdGF0aWNzLnRlYW1zLmNkbi5vZmZpY2UubmV0L2V2ZXJncmVlbi1hc3NldHMvYXBwcy85NWRlNjMzYS0wODNlLTQyZjUtYjQ0NC1hNDI5NWQ4ZTkzMTRfbGFyZ2VJbWFnZS5wbmc/dj0xLjAuNQ==",
    "webUrl": "https://statics.teams.cdn.office.net/evergreen-assets/apps/95de633a-083e-42f5-b444-a4295d8e9314_largeImage.png?v=1.0.5"
}
```

### <a name="example-4-get-outline-icon-of-a-store-teams-app"></a><span data-ttu-id="47995-165">Пример 4. Получить значок плана приложения *Store* Teams</span><span class="sxs-lookup"><span data-stu-id="47995-165">Example 4: Get outline icon of a *store* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="47995-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="47995-166">Request</span></span>

<span data-ttu-id="47995-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47995-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47995-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="47995-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_publicapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/outlineIcon/
```
# <a name="c"></a>[<span data-ttu-id="47995-169">C#</span><span class="sxs-lookup"><span data-stu-id="47995-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamsappicon-outlineicon-publicapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47995-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47995-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamsappicon-outlineicon-publicapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47995-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47995-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamsappicon-outlineicon-publicapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47995-172">Java</span><span class="sxs-lookup"><span data-stu-id="47995-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamsappicon-outlineicon-publicapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="47995-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="47995-173">Response</span></span>

<span data-ttu-id="47995-174">В следующем примере показан ответ для приложения магазина.</span><span class="sxs-lookup"><span data-stu-id="47995-174">The following example shows the response for a store app.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('95de633a-083e-42f5-b444-a4295d8e9314')/appDefinitions('OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk')/outlineIcon/$entity",
    "id": "aHR0cHM6Ly9zdGF0aWNzLnRlYW1zLmNkbi5vZmZpY2UubmV0L2V2ZXJncmVlbi1hc3NldHMvYXBwcy85NWRlNjMzYS0wODNlLTQyZjUtYjQ0NC1hNDI5NWQ4ZTkzMTRfc21hbGxJbWFnZS5wbmc/dj0xLjAuNQ==",
    "webUrl": "https://statics.teams.cdn.office.net/evergreen-assets/apps/95de633a-083e-42f5-b444-a4295d8e9314_smallImage.png?v=1.0.5"
}
```

## <a name="see-also"></a><span data-ttu-id="47995-175">См. также</span><span class="sxs-lookup"><span data-stu-id="47995-175">See also</span></span>

- [<span data-ttu-id="47995-176">Получить контент в значке приложения</span><span class="sxs-lookup"><span data-stu-id="47995-176">Get hosted content in app's icon</span></span>](teamworkhostedcontent-get.md)
- [<span data-ttu-id="47995-177">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="47995-177">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
