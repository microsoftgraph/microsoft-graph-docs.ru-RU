---
title: Get teamworkHostedContent
description: Извлечение содержимого в teamsAppIcon.
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: be9585253f695c9fae9dddf123ad2490d9765da5
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921732"
---
# <a name="get-teamworkhostedcontent"></a><span data-ttu-id="2a7c8-103">Get teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="2a7c8-103">Get teamworkHostedContent</span></span>

<span data-ttu-id="2a7c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a7c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a7c8-105">[Извлечение содержимого в](../resources/teamworkhostedcontent.md) [значке приложения.](../resources/teamsappicon.md)</span><span class="sxs-lookup"><span data-stu-id="2a7c8-105">Retrieve the [hosted content](../resources/teamworkhostedcontent.md) in an [app's icon](../resources/teamsappicon.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a7c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a7c8-106">Permissions</span></span>

<span data-ttu-id="2a7c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a7c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-app-icon-in-app-catalog"></a><span data-ttu-id="2a7c8-109">Разрешения на значок приложения в каталоге приложений</span><span class="sxs-lookup"><span data-stu-id="2a7c8-109">Permissions for app icon in app catalog</span></span>
| <span data-ttu-id="2a7c8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a7c8-110">Permission Type</span></span>                        | <span data-ttu-id="2a7c8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a7c8-111">Permissions (from least to most privileged)</span></span>                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="2a7c8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a7c8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a7c8-113">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="2a7c8-113">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
| <span data-ttu-id="2a7c8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a7c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a7c8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-115">Not supported.</span></span>                                                   |
| <span data-ttu-id="2a7c8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a7c8-116">Application</span></span>                            | <span data-ttu-id="2a7c8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-117">Not supported.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="2a7c8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a7c8-118">HTTP request</span></span>

<span data-ttu-id="2a7c8-119">**Создание содержимого в значке приложения в каталоге приложений**</span><span class="sxs-lookup"><span data-stu-id="2a7c8-119">**Get hosted content in app icon in app catalog**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/$value
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a7c8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a7c8-120">Optional query parameters</span></span>

<span data-ttu-id="2a7c8-121">Эта операция поддерживает `$select` [параметры запроса OData](/graph/query-parameter) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-121">This operation supports the `$select` [OData query parameters](/graph/query-parameter) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a7c8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a7c8-122">Request headers</span></span>

| <span data-ttu-id="2a7c8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a7c8-123">Header</span></span>           | <span data-ttu-id="2a7c8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2a7c8-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="2a7c8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a7c8-125">Authorization</span></span>    | <span data-ttu-id="2a7c8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a7c8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a7c8-128">Request body</span></span>

<span data-ttu-id="2a7c8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a7c8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a7c8-130">Response</span></span>

<span data-ttu-id="2a7c8-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект teamworkHostedContent](../resources/teamworkhostedcontent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-131">If successful, this method returns a `200 OK` response code and a [teamworkHostedContent](../resources/teamworkhostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a7c8-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a7c8-132">Examples</span></span>

### <a name="example-1-get-the-bytes-of-the-hosted-content-of-the-color-icon-of-a-teams-app-in-the-catalog"></a><span data-ttu-id="2a7c8-133">Пример 1. Получить в каталоге биты содержимого значка цвета приложения Teams</span><span class="sxs-lookup"><span data-stu-id="2a7c8-133">Example 1: Get the bytes of the hosted content of the color icon of a Teams app in the catalog</span></span>

#### <a name="request"></a><span data-ttu-id="2a7c8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a7c8-134">Request</span></span>

<span data-ttu-id="2a7c8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a7c8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a7c8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontent_coloricon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/
```
# <a name="c"></a>[<span data-ttu-id="2a7c8-137">C#</span><span class="sxs-lookup"><span data-stu-id="2a7c8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/teamsappicon-get-hostedcontent-coloricon-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a7c8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a7c8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/teamsappicon-get-hostedcontent-coloricon-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a7c8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a7c8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/teamsappicon-get-hostedcontent-coloricon-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a7c8-140">Java</span><span class="sxs-lookup"><span data-stu-id="2a7c8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/teamsappicon-get-hostedcontent-coloricon-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="2a7c8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a7c8-141">Response</span></span>

<span data-ttu-id="2a7c8-142">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-142">The following example shows the response.</span></span>

> <span data-ttu-id="2a7c8-143">**Примечание:** `contentBytes` и `contentType` всегда настроены на нуль.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-143">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/hostedContent/$entity",
    "id": "aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-the-bytes-of-the-hosted-content-of-the-outline-icon-of-a-teams-app-in-the-catalog"></a><span data-ttu-id="2a7c8-144">Пример 2. Получить в каталоге биты содержимого иконки контура приложения Teams</span><span class="sxs-lookup"><span data-stu-id="2a7c8-144">Example 2: Get the bytes of the hosted content of the outline icon of a Teams app in the catalog</span></span>

#### <a name="request"></a><span data-ttu-id="2a7c8-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a7c8-145">Request</span></span>

<span data-ttu-id="2a7c8-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-146">The following is an example of the request.</span></span>

> <span data-ttu-id="2a7c8-147">**Примечание:** Запросы на необработанные значения не поддерживают параметры [запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-147">**Note:** Requests for the raw value does not support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a7c8-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a7c8-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontentbytes_outlineicon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value
```
# <a name="c"></a>[<span data-ttu-id="2a7c8-149">C#</span><span class="sxs-lookup"><span data-stu-id="2a7c8-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/teamsappicon-get-hostedcontentbytes-outlineicon-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a7c8-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a7c8-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/teamsappicon-get-hostedcontentbytes-outlineicon-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a7c8-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a7c8-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/teamsappicon-get-hostedcontentbytes-outlineicon-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a7c8-152">Java</span><span class="sxs-lookup"><span data-stu-id="2a7c8-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/teamsappicon-get-hostedcontentbytes-outlineicon-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a7c8-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a7c8-153">Response</span></span>

<span data-ttu-id="2a7c8-154">Ответ содержит bytes для размещенного контента в теле.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-154">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="2a7c8-155">`content-type` Заглавный заглавник указывает тип содержимого, на который установлено.</span><span class="sxs-lookup"><span data-stu-id="2a7c8-155">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/png
```

## <a name="see-also"></a><span data-ttu-id="2a7c8-156">См. также</span><span class="sxs-lookup"><span data-stu-id="2a7c8-156">See also</span></span>

- [<span data-ttu-id="2a7c8-157">Получить значки приложения Teams</span><span class="sxs-lookup"><span data-stu-id="2a7c8-157">Get icons of a Teams app</span></span>](teamsappicon-get.md)
- [<span data-ttu-id="2a7c8-158">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="2a7c8-158">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
