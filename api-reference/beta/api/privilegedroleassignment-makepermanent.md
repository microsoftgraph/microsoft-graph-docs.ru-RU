---
title: 'Привилежедролеассигнмент: Макеперманент'
description: Выполнение назначения ролей как бессрочного.
localization_priority: Normal
ms.openlocfilehash: 9c6334662cf8496262b49b14ceb3f51f7a4f8dbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538688"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="c6b04-103">Привилежедролеассигнмент: Макеперманент</span><span class="sxs-lookup"><span data-stu-id="c6b04-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6b04-104">Выполнение назначения ролей как бессрочного.</span><span class="sxs-lookup"><span data-stu-id="c6b04-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6b04-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b04-105">Permissions</span></span>
<span data-ttu-id="c6b04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6b04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c6b04-108">Клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="c6b04-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c6b04-109">В противном случае возвращается сообщение об ошибке HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="c6b04-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="c6b04-110">Запрашивающая сторона должна иметь привилегированную роль _администратора ролей_ .</span><span class="sxs-lookup"><span data-stu-id="c6b04-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="c6b04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6b04-111">Permission type</span></span>      | <span data-ttu-id="c6b04-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6b04-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6b04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6b04-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6b04-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6b04-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c6b04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6b04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6b04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b04-116">Not supported.</span></span>    |
|<span data-ttu-id="c6b04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6b04-117">Application</span></span> | <span data-ttu-id="c6b04-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6b04-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6b04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6b04-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="c6b04-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6b04-120">Request headers</span></span>
| <span data-ttu-id="c6b04-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c6b04-121">Name</span></span>       | <span data-ttu-id="c6b04-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c6b04-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6b04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6b04-123">Authorization</span></span>  | <span data-ttu-id="c6b04-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6b04-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6b04-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6b04-126">Request body</span></span>
<span data-ttu-id="c6b04-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c6b04-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c6b04-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="c6b04-128">Parameter</span></span>    | <span data-ttu-id="c6b04-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c6b04-129">Type</span></span>   |<span data-ttu-id="c6b04-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c6b04-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6b04-131">причиной</span><span class="sxs-lookup"><span data-stu-id="c6b04-131">reason</span></span>|<span data-ttu-id="c6b04-132">string</span><span class="sxs-lookup"><span data-stu-id="c6b04-132">string</span></span>|<span data-ttu-id="c6b04-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c6b04-133">Optional.</span></span> <span data-ttu-id="c6b04-134">Причина для совершения звонка.</span><span class="sxs-lookup"><span data-stu-id="c6b04-134">The reason to make this call.</span></span>|
|<span data-ttu-id="c6b04-135">Тиккетнумбер</span><span class="sxs-lookup"><span data-stu-id="c6b04-135">ticketNumber</span></span>|<span data-ttu-id="c6b04-136">string</span><span class="sxs-lookup"><span data-stu-id="c6b04-136">string</span></span>|<span data-ttu-id="c6b04-137">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c6b04-137">Optional.</span></span> <span data-ttu-id="c6b04-138">Регистрационный номер, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c6b04-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="c6b04-139">Тиккетсистем</span><span class="sxs-lookup"><span data-stu-id="c6b04-139">ticketSystem</span></span>|<span data-ttu-id="c6b04-140">string</span><span class="sxs-lookup"><span data-stu-id="c6b04-140">string</span></span>|<span data-ttu-id="c6b04-141">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c6b04-141">Optional.</span></span> <span data-ttu-id="c6b04-142">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="c6b04-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="c6b04-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6b04-143">Response</span></span>

<span data-ttu-id="c6b04-144">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6b04-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6b04-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c6b04-145">Example</span></span>
<span data-ttu-id="c6b04-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c6b04-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c6b04-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6b04-147">Request</span></span>
<span data-ttu-id="c6b04-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6b04-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c6b04-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6b04-149">Response</span></span>
<span data-ttu-id="c6b04-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6b04-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
