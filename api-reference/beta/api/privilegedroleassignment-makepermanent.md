---
title: 'Привилежедролеассигнмент: Макеперманент'
description: Выполнение назначения ролей как бессрочного.
localization_priority: Normal
ms.openlocfilehash: 42425548440d343622cb3d54f4e129ecaa410e1b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268098"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="c9774-103">Привилежедролеассигнмент: Макеперманент</span><span class="sxs-lookup"><span data-stu-id="c9774-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9774-104">Выполнение назначения ролей как бессрочного.</span><span class="sxs-lookup"><span data-stu-id="c9774-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9774-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9774-105">Permissions</span></span>
<span data-ttu-id="c9774-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c9774-108">Клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="c9774-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c9774-109">В противном случае возвращается сообщение об ошибке HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="c9774-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="c9774-110">Запрашивающая сторона должна иметь привилегированную роль _администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="c9774-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="c9774-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9774-111">Permission type</span></span>      | <span data-ttu-id="c9774-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9774-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9774-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9774-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c9774-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c9774-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c9774-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9774-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9774-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9774-116">Not supported.</span></span>    |
|<span data-ttu-id="c9774-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9774-117">Application</span></span> | <span data-ttu-id="c9774-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9774-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9774-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9774-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="c9774-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9774-120">Request headers</span></span>
| <span data-ttu-id="c9774-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c9774-121">Name</span></span>       | <span data-ttu-id="c9774-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c9774-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c9774-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9774-123">Authorization</span></span>  | <span data-ttu-id="c9774-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9774-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9774-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9774-126">Request body</span></span>
<span data-ttu-id="c9774-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c9774-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9774-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="c9774-128">Parameter</span></span>    | <span data-ttu-id="c9774-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c9774-129">Type</span></span>   |<span data-ttu-id="c9774-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c9774-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9774-131">причиной</span><span class="sxs-lookup"><span data-stu-id="c9774-131">reason</span></span>|<span data-ttu-id="c9774-132">string</span><span class="sxs-lookup"><span data-stu-id="c9774-132">string</span></span>|<span data-ttu-id="c9774-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c9774-133">Optional.</span></span> <span data-ttu-id="c9774-134">Причина для совершения звонка.</span><span class="sxs-lookup"><span data-stu-id="c9774-134">The reason to make this call.</span></span>|
|<span data-ttu-id="c9774-135">Тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="c9774-135">ticketNumber</span></span>|<span data-ttu-id="c9774-136">string</span><span class="sxs-lookup"><span data-stu-id="c9774-136">string</span></span>|<span data-ttu-id="c9774-137">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c9774-137">Optional.</span></span> <span data-ttu-id="c9774-138">Регистрационный номер, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c9774-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="c9774-139">Тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="c9774-139">ticketSystem</span></span>|<span data-ttu-id="c9774-140">string</span><span class="sxs-lookup"><span data-stu-id="c9774-140">string</span></span>|<span data-ttu-id="c9774-141">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c9774-141">Optional.</span></span> <span data-ttu-id="c9774-142">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="c9774-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="c9774-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9774-143">Response</span></span>

<span data-ttu-id="c9774-144">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9774-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9774-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c9774-145">Example</span></span>
<span data-ttu-id="c9774-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c9774-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c9774-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9774-147">Request</span></span>
<span data-ttu-id="c9774-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9774-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c9774-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9774-149">Response</span></span>
<span data-ttu-id="c9774-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9774-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c9774-153">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c9774-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c9774-154">C#</span><span class="sxs-lookup"><span data-stu-id="c9774-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_makepermanent-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9774-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="c9774-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_makepermanent-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c9774-156">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c9774-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_makepermanent-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
