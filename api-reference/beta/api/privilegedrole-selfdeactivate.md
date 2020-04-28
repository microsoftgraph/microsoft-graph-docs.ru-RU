---
title: 'Привилежедроле: Селфдеактивате'
description: Деактивация роли, назначенной запрашивающей стороне.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: ea2d8f9a34b2cf4defad6865518044d7908266d4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218747"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="9a463-103">Привилежедроле: Селфдеактивате</span><span class="sxs-lookup"><span data-stu-id="9a463-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="9a463-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a463-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a463-105">Деактивация роли, назначенной запрашивающей стороне.</span><span class="sxs-lookup"><span data-stu-id="9a463-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a463-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a463-106">Permissions</span></span>
<span data-ttu-id="9a463-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9a463-109">Запрашивающая сторона может вызвать ```selfDeactivate``` только назначенную ему роль.</span><span class="sxs-lookup"><span data-stu-id="9a463-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="9a463-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a463-110">Permission type</span></span>      | <span data-ttu-id="9a463-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a463-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a463-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a463-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9a463-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a463-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a463-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a463-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a463-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a463-115">Not supported.</span></span>    |
|<span data-ttu-id="9a463-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a463-116">Application</span></span> | <span data-ttu-id="9a463-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a463-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a463-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a463-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="9a463-119">Обратите ``{id}`` внимание, что это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="9a463-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9a463-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a463-120">Request headers</span></span>
| <span data-ttu-id="9a463-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9a463-121">Name</span></span>       | <span data-ttu-id="9a463-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9a463-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a463-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a463-123">Authorization</span></span>  | <span data-ttu-id="9a463-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a463-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a463-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a463-126">Request body</span></span>
<span data-ttu-id="9a463-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a463-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a463-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a463-128">Response</span></span>

<span data-ttu-id="9a463-129">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9a463-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="9a463-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="9a463-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9a463-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="9a463-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="9a463-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9a463-132">Example</span></span>
<span data-ttu-id="9a463-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9a463-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9a463-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a463-134">Request</span></span>
<span data-ttu-id="9a463-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a463-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a463-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a463-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="9a463-137">C#</span><span class="sxs-lookup"><span data-stu-id="9a463-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a463-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a463-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a463-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a463-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9a463-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a463-140">Response</span></span>
<span data-ttu-id="9a463-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a463-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
