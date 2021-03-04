---
title: Получение privilegedRoleSettings
description: Извлечение параметров ролей для данной роли. Объект privilegedRoleSettings будет возвращен.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 47994dd9f72a880ca1251b8d542fe8c89941a50f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441139"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="e6840-104">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="e6840-104">Get privilegedRoleSettings</span></span>

<span data-ttu-id="e6840-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6840-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6840-106">Извлечение параметров ролей для данной роли.</span><span class="sxs-lookup"><span data-stu-id="e6840-106">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="e6840-107">Объект [privilegedRoleSettings](../resources/privilegedrolesettings.md) будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="e6840-107">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6840-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6840-108">Permissions</span></span>

<span data-ttu-id="e6840-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6840-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e6840-111">У запросителя должна быть одна из следующих ролей: _администратор_ привилегированных _ролей,_ глобальный _администратор,_ администратор безопасности или _читатель безопасности._</span><span class="sxs-lookup"><span data-stu-id="e6840-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="e6840-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6840-112">Permission type</span></span>      | <span data-ttu-id="e6840-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6840-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6840-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6840-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e6840-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6840-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6840-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6840-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6840-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6840-117">Not supported.</span></span>    |
|<span data-ttu-id="e6840-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6840-118">Application</span></span> | <span data-ttu-id="e6840-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6840-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6840-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6840-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6840-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6840-121">Optional query parameters</span></span>
<span data-ttu-id="e6840-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6840-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6840-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6840-123">Request headers</span></span>
| <span data-ttu-id="e6840-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e6840-124">Name</span></span>      |<span data-ttu-id="e6840-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e6840-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6840-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6840-126">Authorization</span></span>  | <span data-ttu-id="e6840-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6840-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6840-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6840-129">Request body</span></span>
<span data-ttu-id="e6840-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6840-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6840-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6840-131">Response</span></span>

<span data-ttu-id="e6840-132">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [privilegedRoleSettings](../resources/privilegedrolesettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e6840-132">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="e6840-133">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="e6840-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e6840-134">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="e6840-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="e6840-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e6840-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6840-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6840-136">Request</span></span>
<span data-ttu-id="e6840-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6840-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6840-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6840-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
# <a name="c"></a>[<span data-ttu-id="e6840-139">C#</span><span class="sxs-lookup"><span data-stu-id="e6840-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrolesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6840-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6840-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrolesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6840-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6840-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrolesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6840-142">Java</span><span class="sxs-lookup"><span data-stu-id="e6840-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrolesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e6840-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6840-143">Response</span></span>
<span data-ttu-id="e6840-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6840-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
