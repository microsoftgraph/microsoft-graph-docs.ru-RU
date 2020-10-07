---
title: Получение privilegedRoleSettings
description: Получение параметров роли для заданной роли. Будет возвращен объект Привилежедролесеттингс.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 6fd8d585f8046d26f971f8598c797eb32e0b7df9
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374380"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="c4ea5-104">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="c4ea5-104">Get privilegedRoleSettings</span></span>

<span data-ttu-id="c4ea5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4ea5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4ea5-106">Получение параметров роли для заданной роли.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-106">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="c4ea5-107">Будет возвращен объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="c4ea5-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4ea5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ea5-108">Permissions</span></span>

<span data-ttu-id="c4ea5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4ea5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c4ea5-111">Запрашивающая сторона должна иметь одну из следующих ролей: _привилегированный администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="c4ea5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4ea5-112">Permission type</span></span>      | <span data-ttu-id="c4ea5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4ea5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4ea5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4ea5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c4ea5-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4ea5-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4ea5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4ea5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4ea5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-117">Not supported.</span></span>    |
|<span data-ttu-id="c4ea5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4ea5-118">Application</span></span> | <span data-ttu-id="c4ea5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4ea5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4ea5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4ea5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c4ea5-121">Optional query parameters</span></span>
<span data-ttu-id="c4ea5-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4ea5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4ea5-123">Request headers</span></span>
| <span data-ttu-id="c4ea5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c4ea5-124">Name</span></span>      |<span data-ttu-id="c4ea5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c4ea5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4ea5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4ea5-126">Authorization</span></span>  | <span data-ttu-id="c4ea5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4ea5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4ea5-129">Request body</span></span>
<span data-ttu-id="c4ea5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4ea5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ea5-131">Response</span></span>

<span data-ttu-id="c4ea5-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролесеттингс](../resources/privilegedrolesettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-132">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="c4ea5-133">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c4ea5-134">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c4ea5-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c4ea5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4ea5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4ea5-136">Request</span></span>
<span data-ttu-id="c4ea5-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c4ea5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ea5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
# <a name="c"></a>[<span data-ttu-id="c4ea5-139">C#</span><span class="sxs-lookup"><span data-stu-id="c4ea5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4ea5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4ea5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4ea5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4ea5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c4ea5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4ea5-142">Response</span></span>
<span data-ttu-id="c4ea5-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4ea5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
