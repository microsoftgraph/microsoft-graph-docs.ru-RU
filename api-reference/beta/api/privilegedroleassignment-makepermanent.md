---
title: 'privilegedRoleAssignment: makePermanent'
description: Сделайте назначение роли постоянным.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a66834f5937b8dea55391553536670ff06ae83c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037377"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="49890-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="49890-103">privilegedRoleAssignment: makePermanent</span></span>

<span data-ttu-id="49890-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49890-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49890-105">Сделайте назначение роли постоянным.</span><span class="sxs-lookup"><span data-stu-id="49890-105">Make the role assignment permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="49890-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49890-106">Permissions</span></span>
<span data-ttu-id="49890-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="49890-109">Клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="49890-109">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="49890-110">В противном случае будет возвращена ошибка http 403 Forbidden.</span><span class="sxs-lookup"><span data-stu-id="49890-110">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="49890-111">Запросчику должна быть роль _администратора привилегированных_ ролей.</span><span class="sxs-lookup"><span data-stu-id="49890-111">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="49890-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49890-112">Permission type</span></span>      | <span data-ttu-id="49890-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49890-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49890-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49890-114">Delegated (work or school account)</span></span> | <span data-ttu-id="49890-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49890-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49890-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49890-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49890-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49890-117">Not supported.</span></span>    |
|<span data-ttu-id="49890-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49890-118">Application</span></span> | <span data-ttu-id="49890-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49890-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49890-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49890-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="49890-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49890-121">Request headers</span></span>
| <span data-ttu-id="49890-122">Имя</span><span class="sxs-lookup"><span data-stu-id="49890-122">Name</span></span>       | <span data-ttu-id="49890-123">Описание</span><span class="sxs-lookup"><span data-stu-id="49890-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="49890-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49890-124">Authorization</span></span>  | <span data-ttu-id="49890-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49890-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49890-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49890-127">Request body</span></span>
<span data-ttu-id="49890-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="49890-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="49890-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="49890-129">Parameter</span></span>    | <span data-ttu-id="49890-130">Тип</span><span class="sxs-lookup"><span data-stu-id="49890-130">Type</span></span>   |<span data-ttu-id="49890-131">Описание</span><span class="sxs-lookup"><span data-stu-id="49890-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49890-132">reason</span><span class="sxs-lookup"><span data-stu-id="49890-132">reason</span></span>|<span data-ttu-id="49890-133">string</span><span class="sxs-lookup"><span data-stu-id="49890-133">string</span></span>|<span data-ttu-id="49890-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="49890-134">Optional.</span></span> <span data-ttu-id="49890-135">Причина для этого вызова.</span><span class="sxs-lookup"><span data-stu-id="49890-135">The reason to make this call.</span></span>|
|<span data-ttu-id="49890-136">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="49890-136">ticketNumber</span></span>|<span data-ttu-id="49890-137">string</span><span class="sxs-lookup"><span data-stu-id="49890-137">string</span></span>|<span data-ttu-id="49890-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="49890-138">Optional.</span></span> <span data-ttu-id="49890-139">Номер билета, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="49890-139">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="49890-140">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="49890-140">ticketSystem</span></span>|<span data-ttu-id="49890-141">string</span><span class="sxs-lookup"><span data-stu-id="49890-141">string</span></span>|<span data-ttu-id="49890-142">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="49890-142">Optional.</span></span> <span data-ttu-id="49890-143">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="49890-143">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="49890-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="49890-144">Response</span></span>

<span data-ttu-id="49890-145">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="49890-145">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49890-146">Пример</span><span class="sxs-lookup"><span data-stu-id="49890-146">Example</span></span>
<span data-ttu-id="49890-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="49890-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="49890-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="49890-148">Request</span></span>
<span data-ttu-id="49890-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49890-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49890-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="49890-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makepermanent"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makePermanent
Content-type: application/json
Content-length: 110

{
  "reason": "reason-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```
# <a name="c"></a>[<span data-ttu-id="49890-151">C#</span><span class="sxs-lookup"><span data-stu-id="49890-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49890-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49890-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49890-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49890-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49890-154">Java</span><span class="sxs-lookup"><span data-stu-id="49890-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makepermanent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="49890-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="49890-155">Response</span></span>
<span data-ttu-id="49890-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49890-156">Here is an example of the response.</span></span> <span data-ttu-id="49890-157">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49890-157">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


