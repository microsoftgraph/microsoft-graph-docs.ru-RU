---
title: 'Привилежедроле: Селфдеактивате'
description: Деактивация роли, назначенной запрашивающей стороне.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 8b721f18978e0512cd81c03fc26de09a6a7505fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035087"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="08780-103">Привилежедроле: Селфдеактивате</span><span class="sxs-lookup"><span data-stu-id="08780-103">privilegedRole: selfDeactivate</span></span>

<span data-ttu-id="08780-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08780-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08780-105">Деактивация роли, назначенной запрашивающей стороне.</span><span class="sxs-lookup"><span data-stu-id="08780-105">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="08780-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08780-106">Permissions</span></span>
<span data-ttu-id="08780-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="08780-109">Запрашивающая сторона может вызвать только ```selfDeactivate``` назначенную ему роль.</span><span class="sxs-lookup"><span data-stu-id="08780-109">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="08780-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08780-110">Permission type</span></span>      | <span data-ttu-id="08780-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08780-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08780-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08780-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08780-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08780-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08780-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08780-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08780-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08780-115">Not supported.</span></span>    |
|<span data-ttu-id="08780-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08780-116">Application</span></span> | <span data-ttu-id="08780-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08780-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="08780-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08780-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="08780-119">Обратите внимание, что ``{id}`` это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="08780-119">Note that ``{id}`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="08780-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08780-120">Request headers</span></span>
| <span data-ttu-id="08780-121">Имя</span><span class="sxs-lookup"><span data-stu-id="08780-121">Name</span></span>       | <span data-ttu-id="08780-122">Описание</span><span class="sxs-lookup"><span data-stu-id="08780-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="08780-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08780-123">Authorization</span></span>  | <span data-ttu-id="08780-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08780-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08780-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08780-126">Request body</span></span>
<span data-ttu-id="08780-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08780-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08780-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="08780-128">Response</span></span>

<span data-ttu-id="08780-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08780-129">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="08780-130">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="08780-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="08780-131">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="08780-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="08780-132">Пример</span><span class="sxs-lookup"><span data-stu-id="08780-132">Example</span></span>
<span data-ttu-id="08780-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="08780-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="08780-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="08780-134">Request</span></span>
<span data-ttu-id="08780-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08780-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="08780-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="08780-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="c"></a>[<span data-ttu-id="08780-137">C#</span><span class="sxs-lookup"><span data-stu-id="08780-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08780-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08780-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08780-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08780-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08780-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="08780-140">Response</span></span>
<span data-ttu-id="08780-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08780-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


