---
title: Get teamsAppIcon
description: Извлечение значка, связанного с определенным определением приложения Teams.
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1ccada523f670df173304fafd43747a63444e7e2
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882704"
---
# <a name="get-teamsappicon"></a><span data-ttu-id="2724f-103">Get teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="2724f-103">Get teamsAppIcon</span></span>

<span data-ttu-id="2724f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2724f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2724f-105">[Извлечение значка приложения Teams,](../resources/teamsappicon.md) связанного с определенным [определением](../resources/teamsappdefinition.md) [приложения.](../resources/teamsapp.md)</span><span class="sxs-lookup"><span data-stu-id="2724f-105">Retrieve a [Teams app icon](../resources/teamsappicon.md) associated with a specific [definition](../resources/teamsappdefinition.md) of an [app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2724f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2724f-106">Permissions</span></span>

<span data-ttu-id="2724f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2724f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2724f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2724f-109">Permission Type</span></span>                        | <span data-ttu-id="2724f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2724f-110">Permissions (from least to most privileged)</span></span>                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="2724f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2724f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2724f-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="2724f-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
| <span data-ttu-id="2724f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2724f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2724f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2724f-114">Not supported.</span></span>                                                   |
| <span data-ttu-id="2724f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2724f-115">Application</span></span>                            | <span data-ttu-id="2724f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2724f-116">Not supported.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="2724f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2724f-117">HTTP request</span></span>

<span data-ttu-id="2724f-118">**Получить значок цвета определения приложения Teams**</span><span class="sxs-lookup"><span data-stu-id="2724f-118">**Get color icon of a Teams app definition**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon
```

<span data-ttu-id="2724f-119">**Получить значок контура определения приложения Teams**</span><span class="sxs-lookup"><span data-stu-id="2724f-119">**Get outline icon of a Teams app definition**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2724f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2724f-120">Optional query parameters</span></span>

<span data-ttu-id="2724f-121">Эта операция поддерживает параметры `$select` `$expand` [запроса oData и OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2724f-121">This operation supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2724f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2724f-122">Request headers</span></span>

| <span data-ttu-id="2724f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2724f-123">Header</span></span>           | <span data-ttu-id="2724f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2724f-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="2724f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2724f-125">Authorization</span></span>    | <span data-ttu-id="2724f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2724f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2724f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2724f-128">Request body</span></span>

<span data-ttu-id="2724f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2724f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2724f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2724f-130">Response</span></span>

<span data-ttu-id="2724f-131">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [teamsAppIcon](../resources/teamsappicon.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2724f-131">If successful, this method returns a `200 OK` response code and a [teamsAppIcon](../resources/teamsappicon.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2724f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2724f-132">Examples</span></span>

### <a name="example-1-get-color-icon-of-a-custom-teams-app"></a><span data-ttu-id="2724f-133">Пример 1. Получить значок цвета *настраиваемого* приложения Teams</span><span class="sxs-lookup"><span data-stu-id="2724f-133">Example 1: Get color icon of a *custom* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="2724f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2724f-134">Request</span></span>

<span data-ttu-id="2724f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2724f-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_coloricon_customapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon
```

#### <a name="response"></a><span data-ttu-id="2724f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2724f-136">Response</span></span>

<span data-ttu-id="2724f-137">В следующем примере показан ответ для организационного приложения.</span><span class="sxs-lookup"><span data-stu-id="2724f-137">The following example shows the response for an organizational app.</span></span> 
> <span data-ttu-id="2724f-138">**Примечание.** Для доступа к [фактическому](teamworkhostedcontent-get.md) изображению значка настраиваемого приложения требуется задать маркер Microsoft Graph в запросе.</span><span class="sxs-lookup"><span data-stu-id="2724f-138">**Note**: Accessing the actual [image of the custom app's icon](teamworkhostedcontent-get.md) requires a Microsoft Graph token to be set on the request.</span></span>

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

### <a name="example-2-get-outline-icon-of-a-custom-teams-app"></a><span data-ttu-id="2724f-139">Пример 2. Получить значок контура *настраиваемого* приложения Teams</span><span class="sxs-lookup"><span data-stu-id="2724f-139">Example 2: Get outline icon of a *custom* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="2724f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2724f-140">Request</span></span>

<span data-ttu-id="2724f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2724f-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_customapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon
```

#### <a name="response"></a><span data-ttu-id="2724f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2724f-142">Response</span></span>

<span data-ttu-id="2724f-143">В следующем примере показан ответ для организационного приложения.</span><span class="sxs-lookup"><span data-stu-id="2724f-143">The following example shows the response for an organizational app.</span></span> 
> <span data-ttu-id="2724f-144">**Примечание.** Для доступа к [фактическому](teamworkhostedcontent-get.md) изображению значка настраиваемого приложения требуется задать маркер Microsoft Graph в запросе.</span><span class="sxs-lookup"><span data-stu-id="2724f-144">**Note**:  Accessing the actual [image of the custom app's icon](teamworkhostedcontent-get.md) requires a Microsoft Graph token to be set on the request.</span></span>


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


### <a name="example-3-get-color-icon-of-a-store-teams-app"></a><span data-ttu-id="2724f-145">Пример 3. Получить значок цвета приложения *Store* Teams</span><span class="sxs-lookup"><span data-stu-id="2724f-145">Example 3: Get color icon of a *store* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="2724f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="2724f-146">Request</span></span>

<span data-ttu-id="2724f-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2724f-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_publicapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/colorIcon/
```


#### <a name="response"></a><span data-ttu-id="2724f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="2724f-148">Response</span></span>

<span data-ttu-id="2724f-149">В следующем примере показан ответ для приложения магазина.</span><span class="sxs-lookup"><span data-stu-id="2724f-149">The following example shows the response for a store app.</span></span>

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

### <a name="example-4-get-outline-icon-of-a-store-teams-app"></a><span data-ttu-id="2724f-150">Пример 4. Получить значок плана приложения *Store* Teams</span><span class="sxs-lookup"><span data-stu-id="2724f-150">Example 4: Get outline icon of a *store* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="2724f-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="2724f-151">Request</span></span>

<span data-ttu-id="2724f-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2724f-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_publicapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/outlineIcon/
```


#### <a name="response"></a><span data-ttu-id="2724f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2724f-153">Response</span></span>

<span data-ttu-id="2724f-154">В следующем примере показан ответ для приложения магазина.</span><span class="sxs-lookup"><span data-stu-id="2724f-154">The following example shows the response for a store app.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2724f-155">См. также</span><span class="sxs-lookup"><span data-stu-id="2724f-155">See also</span></span>

- [<span data-ttu-id="2724f-156">Получить контент в значке приложения</span><span class="sxs-lookup"><span data-stu-id="2724f-156">Get hosted content in app's icon</span></span>](teamworkhostedcontent-get.md)
- [<span data-ttu-id="2724f-157">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="2724f-157">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
