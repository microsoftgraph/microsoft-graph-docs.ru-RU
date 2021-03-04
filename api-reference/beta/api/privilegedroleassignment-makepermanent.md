---
title: 'privilegedRoleAssignment: makePermanent'
description: Сделайте назначение роли постоянным.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: c457cc3c70e1a3f7cafec9a929c68ed3b7fddcea
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441202"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="7b82f-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="7b82f-103">privilegedRoleAssignment: makePermanent</span></span>

<span data-ttu-id="7b82f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b82f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b82f-105">Сделайте назначение роли постоянным.</span><span class="sxs-lookup"><span data-stu-id="7b82f-105">Make the role assignment permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b82f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b82f-106">Permissions</span></span>
<span data-ttu-id="7b82f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b82f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7b82f-109">Клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="7b82f-109">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7b82f-110">В противном случае будет возвращена ошибка http 403 Forbidden.</span><span class="sxs-lookup"><span data-stu-id="7b82f-110">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="7b82f-111">Запросчику должна быть роль _администратора привилегированных_ ролей.</span><span class="sxs-lookup"><span data-stu-id="7b82f-111">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="7b82f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b82f-112">Permission type</span></span>      | <span data-ttu-id="7b82f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b82f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b82f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b82f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7b82f-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b82f-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b82f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b82f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b82f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b82f-117">Not supported.</span></span>    |
|<span data-ttu-id="7b82f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b82f-118">Application</span></span> | <span data-ttu-id="7b82f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b82f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b82f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b82f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="7b82f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b82f-121">Request headers</span></span>
| <span data-ttu-id="7b82f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7b82f-122">Name</span></span>       | <span data-ttu-id="7b82f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7b82f-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7b82f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b82f-124">Authorization</span></span>  | <span data-ttu-id="7b82f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b82f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b82f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b82f-127">Request body</span></span>
<span data-ttu-id="7b82f-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7b82f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7b82f-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="7b82f-129">Parameter</span></span>    | <span data-ttu-id="7b82f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7b82f-130">Type</span></span>   |<span data-ttu-id="7b82f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7b82f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b82f-132">reason</span><span class="sxs-lookup"><span data-stu-id="7b82f-132">reason</span></span>|<span data-ttu-id="7b82f-133">string</span><span class="sxs-lookup"><span data-stu-id="7b82f-133">string</span></span>|<span data-ttu-id="7b82f-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7b82f-134">Optional.</span></span> <span data-ttu-id="7b82f-135">Причина для этого вызова.</span><span class="sxs-lookup"><span data-stu-id="7b82f-135">The reason to make this call.</span></span>|
|<span data-ttu-id="7b82f-136">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="7b82f-136">ticketNumber</span></span>|<span data-ttu-id="7b82f-137">string</span><span class="sxs-lookup"><span data-stu-id="7b82f-137">string</span></span>|<span data-ttu-id="7b82f-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7b82f-138">Optional.</span></span> <span data-ttu-id="7b82f-139">Номер билета, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="7b82f-139">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="7b82f-140">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="7b82f-140">ticketSystem</span></span>|<span data-ttu-id="7b82f-141">string</span><span class="sxs-lookup"><span data-stu-id="7b82f-141">string</span></span>|<span data-ttu-id="7b82f-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7b82f-142">Optional.</span></span> <span data-ttu-id="7b82f-143">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="7b82f-143">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="7b82f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b82f-144">Response</span></span>

<span data-ttu-id="7b82f-145">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7b82f-145">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b82f-146">Пример</span><span class="sxs-lookup"><span data-stu-id="7b82f-146">Example</span></span>
<span data-ttu-id="7b82f-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7b82f-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7b82f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b82f-148">Request</span></span>
<span data-ttu-id="7b82f-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b82f-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b82f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b82f-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7b82f-151">C#</span><span class="sxs-lookup"><span data-stu-id="7b82f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b82f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b82f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b82f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b82f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b82f-154">Java</span><span class="sxs-lookup"><span data-stu-id="7b82f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makepermanent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7b82f-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b82f-155">Response</span></span>
<span data-ttu-id="7b82f-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b82f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


