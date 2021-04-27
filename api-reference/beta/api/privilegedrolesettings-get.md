---
title: Получение privilegedRoleSettings
description: Извлечение параметров ролей для данной роли. Объект privilegedRoleSettings будет возвращен.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 73c2a01c171ec39f2702b5bf9ce6a3138a93456b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052889"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="dd778-104">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="dd778-104">Get privilegedRoleSettings</span></span>

<span data-ttu-id="dd778-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd778-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd778-106">Извлечение параметров ролей для данной роли.</span><span class="sxs-lookup"><span data-stu-id="dd778-106">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="dd778-107">Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="dd778-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd778-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd778-108">Permissions</span></span>

<span data-ttu-id="dd778-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd778-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dd778-111">У запросителя должна быть одна из следующих ролей: _администратор_ привилегированных _ролей,_ глобальный _администратор,_ администратор безопасности или _читатель безопасности._</span><span class="sxs-lookup"><span data-stu-id="dd778-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="dd778-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd778-112">Permission type</span></span>      | <span data-ttu-id="dd778-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd778-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd778-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd778-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dd778-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd778-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd778-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd778-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd778-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd778-117">Not supported.</span></span>    |
|<span data-ttu-id="dd778-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd778-118">Application</span></span> | <span data-ttu-id="dd778-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd778-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd778-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd778-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd778-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd778-121">Optional query parameters</span></span>
<span data-ttu-id="dd778-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd778-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd778-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd778-123">Request headers</span></span>
| <span data-ttu-id="dd778-124">Имя</span><span class="sxs-lookup"><span data-stu-id="dd778-124">Name</span></span>      |<span data-ttu-id="dd778-125">Описание</span><span class="sxs-lookup"><span data-stu-id="dd778-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd778-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd778-126">Authorization</span></span>  | <span data-ttu-id="dd778-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd778-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd778-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd778-129">Request body</span></span>
<span data-ttu-id="dd778-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd778-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd778-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd778-131">Response</span></span>

<span data-ttu-id="dd778-132">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [privilegedRoleSettings](../resources/privilegedrolesettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd778-132">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="dd778-133">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="dd778-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="dd778-134">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="dd778-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="dd778-135">Пример</span><span class="sxs-lookup"><span data-stu-id="dd778-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd778-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd778-136">Request</span></span>
<span data-ttu-id="dd778-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd778-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd778-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd778-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
# <a name="c"></a>[<span data-ttu-id="dd778-139">C#</span><span class="sxs-lookup"><span data-stu-id="dd778-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd778-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd778-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd778-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd778-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd778-142">Java</span><span class="sxs-lookup"><span data-stu-id="dd778-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd778-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd778-143">Response</span></span>
<span data-ttu-id="dd778-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd778-144">Here is an example of the response.</span></span> <span data-ttu-id="dd778-145">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dd778-145">Note: The response object shown here might be shortened for readability.</span></span>
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
