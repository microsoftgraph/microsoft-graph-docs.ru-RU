---
title: 'privilegedRoleAssignment: makeEligible'
description: Сделайте назначение роли подходящим.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 97daaea03d58d73ab687380dd221d3e300b446c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037456"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="d2a42-103">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="d2a42-103">privilegedRoleAssignment: makeEligible</span></span>

<span data-ttu-id="d2a42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2a42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2a42-105">Сделайте назначение роли подходящим.</span><span class="sxs-lookup"><span data-stu-id="d2a42-105">Make the role assignment eligible.</span></span> <span data-ttu-id="d2a42-106">Если назначение роли уже имеет право на выполнение перед вызовом, оно ничего не делает.</span><span class="sxs-lookup"><span data-stu-id="d2a42-106">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="d2a42-107">Если назначение роли является постоянным, а запросчик отличается от целевого пользователя, назначение роли становится подходящим и роль будет отключена для целевого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d2a42-107">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="d2a42-108">Если запрашиватель является целевым пользователем, а роль — администратором безопасности или администратором привилегированных ролей, роль активируется с истечением срока действия по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d2a42-108">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2a42-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2a42-109">Permissions</span></span>
<span data-ttu-id="d2a42-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2a42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d2a42-112">Запросчику должна быть роль _администратора привилегированных_ ролей.</span><span class="sxs-lookup"><span data-stu-id="d2a42-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="d2a42-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2a42-113">Permission type</span></span>      | <span data-ttu-id="d2a42-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2a42-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2a42-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2a42-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d2a42-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2a42-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2a42-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2a42-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2a42-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2a42-118">Not supported.</span></span>    |
|<span data-ttu-id="d2a42-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2a42-119">Application</span></span> | <span data-ttu-id="d2a42-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2a42-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2a42-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2a42-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="d2a42-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2a42-122">Request headers</span></span>
| <span data-ttu-id="d2a42-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d2a42-123">Name</span></span>       | <span data-ttu-id="d2a42-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d2a42-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d2a42-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2a42-125">Authorization</span></span>  | <span data-ttu-id="d2a42-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2a42-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2a42-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2a42-128">Request body</span></span>
<span data-ttu-id="d2a42-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2a42-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2a42-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2a42-130">Response</span></span>

<span data-ttu-id="d2a42-131">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2a42-131">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="d2a42-132">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="d2a42-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d2a42-133">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="d2a42-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d2a42-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d2a42-134">Example</span></span>
<span data-ttu-id="d2a42-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d2a42-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2a42-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2a42-136">Request</span></span>
<span data-ttu-id="d2a42-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2a42-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2a42-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2a42-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="c"></a>[<span data-ttu-id="d2a42-139">C#</span><span class="sxs-lookup"><span data-stu-id="d2a42-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2a42-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2a42-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2a42-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2a42-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2a42-142">Java</span><span class="sxs-lookup"><span data-stu-id="d2a42-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makeeligible-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d2a42-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2a42-143">Response</span></span>
<span data-ttu-id="d2a42-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2a42-144">Here is an example of the response.</span></span> <span data-ttu-id="d2a42-145">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d2a42-145">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


