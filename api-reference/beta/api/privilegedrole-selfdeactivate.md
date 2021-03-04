---
title: 'privilegedRole: selfDeactivate'
description: Деактивация роли, назначенной запрашивающей стороне.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a50f74e928d95ba5bce5e39dc61febb30f9d67b7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441286"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="ae090-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="ae090-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="ae090-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae090-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae090-105">Деактивация роли, назначенной запрашивающей стороне.</span><span class="sxs-lookup"><span data-stu-id="ae090-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae090-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae090-106">Permissions</span></span>
<span data-ttu-id="ae090-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ae090-109">Запросчик может вызывать только назначенную ему ```selfDeactivate``` роль.</span><span class="sxs-lookup"><span data-stu-id="ae090-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="ae090-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae090-110">Permission type</span></span>      | <span data-ttu-id="ae090-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae090-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae090-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae090-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ae090-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae090-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae090-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae090-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae090-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae090-115">Not supported.</span></span>    |
|<span data-ttu-id="ae090-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae090-116">Application</span></span> | <span data-ttu-id="ae090-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae090-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae090-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae090-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="ae090-119">Обратите ``{id}`` внимание, что это целевой id роли.</span><span class="sxs-lookup"><span data-stu-id="ae090-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ae090-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae090-120">Request headers</span></span>
| <span data-ttu-id="ae090-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ae090-121">Name</span></span>       | <span data-ttu-id="ae090-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ae090-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae090-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae090-123">Authorization</span></span>  | <span data-ttu-id="ae090-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae090-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae090-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae090-126">Request body</span></span>
<span data-ttu-id="ae090-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae090-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae090-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae090-128">Response</span></span>

<span data-ttu-id="ae090-129">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ae090-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="ae090-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="ae090-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ae090-131">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="ae090-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ae090-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ae090-132">Example</span></span>
<span data-ttu-id="ae090-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ae090-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae090-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae090-134">Request</span></span>
<span data-ttu-id="ae090-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae090-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae090-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae090-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="ae090-137">C#</span><span class="sxs-lookup"><span data-stu-id="ae090-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae090-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae090-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae090-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae090-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae090-140">Java</span><span class="sxs-lookup"><span data-stu-id="ae090-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfdeactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ae090-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae090-141">Response</span></span>
<span data-ttu-id="ae090-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae090-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


