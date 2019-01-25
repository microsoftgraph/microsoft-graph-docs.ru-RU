---
title: 'privilegedRoleAssignment: makePermanent'
description: Сделайте как постоянное назначение ролей.
localization_priority: Normal
ms.openlocfilehash: 9c6334662cf8496262b49b14ceb3f51f7a4f8dbc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511396"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="1c44c-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="1c44c-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c44c-104">Сделайте как постоянное назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="1c44c-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c44c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c44c-105">Permissions</span></span>
<span data-ttu-id="1c44c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c44c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1c44c-108">Клиента должен быть зарегистрированы и для управления персональными данными.</span><span class="sxs-lookup"><span data-stu-id="1c44c-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="1c44c-109">В противном случае будет возвращена ошибка HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="1c44c-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="1c44c-110">Запрашивающая сторона должна иметь роль _Привилегированной роль администратора_ .</span><span class="sxs-lookup"><span data-stu-id="1c44c-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="1c44c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c44c-111">Permission type</span></span>      | <span data-ttu-id="1c44c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c44c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c44c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c44c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1c44c-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c44c-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1c44c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c44c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c44c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c44c-116">Not supported.</span></span>    |
|<span data-ttu-id="1c44c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c44c-117">Application</span></span> | <span data-ttu-id="1c44c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c44c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c44c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c44c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="1c44c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c44c-120">Request headers</span></span>
| <span data-ttu-id="1c44c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1c44c-121">Name</span></span>       | <span data-ttu-id="1c44c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1c44c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1c44c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c44c-123">Authorization</span></span>  | <span data-ttu-id="1c44c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c44c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c44c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c44c-126">Request body</span></span>
<span data-ttu-id="1c44c-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1c44c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c44c-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="1c44c-128">Parameter</span></span>    | <span data-ttu-id="1c44c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1c44c-129">Type</span></span>   |<span data-ttu-id="1c44c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1c44c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c44c-131">Причина</span><span class="sxs-lookup"><span data-stu-id="1c44c-131">reason</span></span>|<span data-ttu-id="1c44c-132">string</span><span class="sxs-lookup"><span data-stu-id="1c44c-132">string</span></span>|<span data-ttu-id="1c44c-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1c44c-133">Optional.</span></span> <span data-ttu-id="1c44c-134">Причиной, чтобы сделать этот вызов.</span><span class="sxs-lookup"><span data-stu-id="1c44c-134">The reason to make this call.</span></span>|
|<span data-ttu-id="1c44c-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="1c44c-135">ticketNumber</span></span>|<span data-ttu-id="1c44c-136">string</span><span class="sxs-lookup"><span data-stu-id="1c44c-136">string</span></span>|<span data-ttu-id="1c44c-137">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1c44c-137">Optional.</span></span> <span data-ttu-id="1c44c-138">Номер билетов, который связан с этой операции.</span><span class="sxs-lookup"><span data-stu-id="1c44c-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="1c44c-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="1c44c-139">ticketSystem</span></span>|<span data-ttu-id="1c44c-140">string</span><span class="sxs-lookup"><span data-stu-id="1c44c-140">string</span></span>|<span data-ttu-id="1c44c-141">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1c44c-141">Optional.</span></span> <span data-ttu-id="1c44c-142">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="1c44c-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="1c44c-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c44c-143">Response</span></span>

<span data-ttu-id="1c44c-144">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1c44c-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c44c-145">Пример</span><span class="sxs-lookup"><span data-stu-id="1c44c-145">Example</span></span>
<span data-ttu-id="1c44c-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1c44c-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1c44c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c44c-147">Request</span></span>
<span data-ttu-id="1c44c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c44c-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1c44c-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c44c-149">Response</span></span>
<span data-ttu-id="1c44c-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1c44c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
