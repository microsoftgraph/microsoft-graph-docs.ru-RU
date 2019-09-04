---
title: Получение privilegedRoleSettings
description: Получение параметров роли для заданной роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 82ce3cc2d7a8fab58b8fb8243a791823567b1477
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723422"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="20d5c-104">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="20d5c-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20d5c-105">Получение параметров роли для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="20d5c-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="20d5c-106">Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="20d5c-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="20d5c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20d5c-107">Permissions</span></span>

<span data-ttu-id="20d5c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20d5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="20d5c-110">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="20d5c-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="20d5c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20d5c-111">Permission type</span></span>      | <span data-ttu-id="20d5c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20d5c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20d5c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20d5c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="20d5c-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20d5c-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20d5c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20d5c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20d5c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20d5c-116">Not supported.</span></span>    |
|<span data-ttu-id="20d5c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20d5c-117">Application</span></span> | <span data-ttu-id="20d5c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20d5c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20d5c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20d5c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20d5c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20d5c-120">Optional query parameters</span></span>
<span data-ttu-id="20d5c-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="20d5c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20d5c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20d5c-122">Request headers</span></span>
| <span data-ttu-id="20d5c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="20d5c-123">Name</span></span>      |<span data-ttu-id="20d5c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="20d5c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="20d5c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20d5c-125">Authorization</span></span>  | <span data-ttu-id="20d5c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20d5c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20d5c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20d5c-128">Request body</span></span>
<span data-ttu-id="20d5c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20d5c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20d5c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="20d5c-130">Response</span></span>

<span data-ttu-id="20d5c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20d5c-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="20d5c-132">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="20d5c-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="20d5c-133">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="20d5c-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="20d5c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="20d5c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20d5c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="20d5c-135">Request</span></span>
<span data-ttu-id="20d5c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20d5c-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="20d5c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="20d5c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20d5c-138">C#</span><span class="sxs-lookup"><span data-stu-id="20d5c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20d5c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20d5c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20d5c-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="20d5c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="20d5c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="20d5c-141">Response</span></span>
<span data-ttu-id="20d5c-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20d5c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 228

{
  "minElevationDuration": "2016-10-19T10:37:00Z",
  "maxElavationDuration": "2016-10-19T10:37:00Z",
  "elevationDuration": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
