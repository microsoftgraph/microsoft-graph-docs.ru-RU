---
title: 'Привилежедролеассигнмент: Макеперманент'
description: Выполнение назначения ролей как бессрочного.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d1d8995f8effa376b13393e59db30831d9ac49d0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412693"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="56805-103">Привилежедролеассигнмент: Макеперманент</span><span class="sxs-lookup"><span data-stu-id="56805-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56805-104">Выполнение назначения ролей как бессрочного.</span><span class="sxs-lookup"><span data-stu-id="56805-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="56805-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56805-105">Permissions</span></span>
<span data-ttu-id="56805-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56805-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="56805-108">Клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="56805-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="56805-109">В противном случае возвращается сообщение об ошибке HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="56805-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="56805-110">Запрашивающая сторона должна иметь привилегированную роль _администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="56805-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="56805-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56805-111">Permission type</span></span>      | <span data-ttu-id="56805-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56805-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56805-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56805-113">Delegated (work or school account)</span></span> | <span data-ttu-id="56805-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56805-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56805-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56805-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56805-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56805-116">Not supported.</span></span>    |
|<span data-ttu-id="56805-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56805-117">Application</span></span> | <span data-ttu-id="56805-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56805-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56805-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56805-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="56805-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56805-120">Request headers</span></span>
| <span data-ttu-id="56805-121">Имя</span><span class="sxs-lookup"><span data-stu-id="56805-121">Name</span></span>       | <span data-ttu-id="56805-122">Описание</span><span class="sxs-lookup"><span data-stu-id="56805-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56805-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56805-123">Authorization</span></span>  | <span data-ttu-id="56805-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56805-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56805-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56805-126">Request body</span></span>
<span data-ttu-id="56805-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="56805-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="56805-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="56805-128">Parameter</span></span>    | <span data-ttu-id="56805-129">Тип</span><span class="sxs-lookup"><span data-stu-id="56805-129">Type</span></span>   |<span data-ttu-id="56805-130">Описание</span><span class="sxs-lookup"><span data-stu-id="56805-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56805-131">причиной</span><span class="sxs-lookup"><span data-stu-id="56805-131">reason</span></span>|<span data-ttu-id="56805-132">string</span><span class="sxs-lookup"><span data-stu-id="56805-132">string</span></span>|<span data-ttu-id="56805-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="56805-133">Optional.</span></span> <span data-ttu-id="56805-134">Причина для совершения звонка.</span><span class="sxs-lookup"><span data-stu-id="56805-134">The reason to make this call.</span></span>|
|<span data-ttu-id="56805-135">тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="56805-135">ticketNumber</span></span>|<span data-ttu-id="56805-136">string</span><span class="sxs-lookup"><span data-stu-id="56805-136">string</span></span>|<span data-ttu-id="56805-137">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="56805-137">Optional.</span></span> <span data-ttu-id="56805-138">Регистрационный номер, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="56805-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="56805-139">тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="56805-139">ticketSystem</span></span>|<span data-ttu-id="56805-140">string</span><span class="sxs-lookup"><span data-stu-id="56805-140">string</span></span>|<span data-ttu-id="56805-141">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="56805-141">Optional.</span></span> <span data-ttu-id="56805-142">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="56805-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="56805-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="56805-143">Response</span></span>

<span data-ttu-id="56805-144">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56805-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56805-145">Пример</span><span class="sxs-lookup"><span data-stu-id="56805-145">Example</span></span>
<span data-ttu-id="56805-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="56805-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="56805-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="56805-147">Request</span></span>
<span data-ttu-id="56805-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56805-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="56805-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="56805-149">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="56805-150">C#</span><span class="sxs-lookup"><span data-stu-id="56805-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56805-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56805-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56805-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="56805-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="56805-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="56805-153">Response</span></span>
<span data-ttu-id="56805-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56805-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
