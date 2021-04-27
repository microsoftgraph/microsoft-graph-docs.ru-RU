---
title: 'privilegedRole: selfDeactivate'
description: Деактивация роли, назначенной запрашивающей стороне.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 5c2b2bbd11308f4a593dce3709581b8facb8516d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055248"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="49ddc-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="49ddc-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="49ddc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49ddc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49ddc-105">Деактивация роли, назначенной запрашивающей стороне.</span><span class="sxs-lookup"><span data-stu-id="49ddc-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="49ddc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49ddc-106">Permissions</span></span>
<span data-ttu-id="49ddc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="49ddc-109">Запросчик может вызывать только назначенную ему ```selfDeactivate``` роль.</span><span class="sxs-lookup"><span data-stu-id="49ddc-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="49ddc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49ddc-110">Permission type</span></span>      | <span data-ttu-id="49ddc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49ddc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49ddc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49ddc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49ddc-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49ddc-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49ddc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49ddc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49ddc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49ddc-115">Not supported.</span></span>    |
|<span data-ttu-id="49ddc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49ddc-116">Application</span></span> | <span data-ttu-id="49ddc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49ddc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49ddc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49ddc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="49ddc-119">Обратите ``{id}`` внимание, что это целевой id роли.</span><span class="sxs-lookup"><span data-stu-id="49ddc-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="49ddc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49ddc-120">Request headers</span></span>
| <span data-ttu-id="49ddc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="49ddc-121">Name</span></span>       | <span data-ttu-id="49ddc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="49ddc-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49ddc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49ddc-123">Authorization</span></span>  | <span data-ttu-id="49ddc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49ddc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49ddc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49ddc-126">Request body</span></span>
<span data-ttu-id="49ddc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49ddc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49ddc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="49ddc-128">Response</span></span>

<span data-ttu-id="49ddc-129">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="49ddc-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="49ddc-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="49ddc-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="49ddc-131">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="49ddc-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="49ddc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="49ddc-132">Example</span></span>
<span data-ttu-id="49ddc-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="49ddc-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49ddc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="49ddc-134">Request</span></span>
<span data-ttu-id="49ddc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49ddc-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49ddc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="49ddc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="49ddc-137">C#</span><span class="sxs-lookup"><span data-stu-id="49ddc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49ddc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49ddc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49ddc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49ddc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49ddc-140">Java</span><span class="sxs-lookup"><span data-stu-id="49ddc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfdeactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49ddc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="49ddc-141">Response</span></span>
<span data-ttu-id="49ddc-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49ddc-142">Here is an example of the response.</span></span> <span data-ttu-id="49ddc-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49ddc-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


