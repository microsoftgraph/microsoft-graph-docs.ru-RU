---
title: 'privilegedRoleAssignment: makePermanent'
description: Сделайте как постоянное назначение ролей.
localization_priority: Normal
ms.openlocfilehash: c2c834454f7c6c7bd931b6985f5b35b92e48096d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849695"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="74e5c-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="74e5c-103">privilegedRoleAssignment: makePermanent</span></span>

> <span data-ttu-id="74e5c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74e5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74e5c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74e5c-106">Сделайте как постоянное назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="74e5c-106">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="74e5c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74e5c-107">Permissions</span></span>
<span data-ttu-id="74e5c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74e5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="74e5c-110">Клиента должен быть зарегистрированы и для управления персональными данными.</span><span class="sxs-lookup"><span data-stu-id="74e5c-110">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="74e5c-111">В противном случае будет возвращена ошибка HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="74e5c-111">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="74e5c-112">Запрашивающая сторона должна иметь роль _Привилегированной роль администратора_ .</span><span class="sxs-lookup"><span data-stu-id="74e5c-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="74e5c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74e5c-113">Permission type</span></span>      | <span data-ttu-id="74e5c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74e5c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74e5c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74e5c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="74e5c-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74e5c-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="74e5c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74e5c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e5c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e5c-118">Not supported.</span></span>    |
|<span data-ttu-id="74e5c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74e5c-119">Application</span></span> | <span data-ttu-id="74e5c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74e5c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74e5c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74e5c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="74e5c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74e5c-122">Request headers</span></span>
| <span data-ttu-id="74e5c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="74e5c-123">Name</span></span>       | <span data-ttu-id="74e5c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="74e5c-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="74e5c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74e5c-125">Authorization</span></span>  | <span data-ttu-id="74e5c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74e5c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74e5c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74e5c-128">Request body</span></span>
<span data-ttu-id="74e5c-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="74e5c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74e5c-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="74e5c-130">Parameter</span></span>    | <span data-ttu-id="74e5c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74e5c-131">Type</span></span>   |<span data-ttu-id="74e5c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74e5c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74e5c-133">Причина</span><span class="sxs-lookup"><span data-stu-id="74e5c-133">reason</span></span>|<span data-ttu-id="74e5c-134">string</span><span class="sxs-lookup"><span data-stu-id="74e5c-134">string</span></span>|<span data-ttu-id="74e5c-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="74e5c-135">Optional.</span></span> <span data-ttu-id="74e5c-136">Причиной, чтобы сделать этот вызов.</span><span class="sxs-lookup"><span data-stu-id="74e5c-136">The reason to make this call.</span></span>|
|<span data-ttu-id="74e5c-137">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="74e5c-137">ticketNumber</span></span>|<span data-ttu-id="74e5c-138">string</span><span class="sxs-lookup"><span data-stu-id="74e5c-138">string</span></span>|<span data-ttu-id="74e5c-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="74e5c-139">Optional.</span></span> <span data-ttu-id="74e5c-140">Номер билетов, который связан с этой операции.</span><span class="sxs-lookup"><span data-stu-id="74e5c-140">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="74e5c-141">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="74e5c-141">ticketSystem</span></span>|<span data-ttu-id="74e5c-142">string</span><span class="sxs-lookup"><span data-stu-id="74e5c-142">string</span></span>|<span data-ttu-id="74e5c-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="74e5c-143">Optional.</span></span> <span data-ttu-id="74e5c-144">Система билетов.</span><span class="sxs-lookup"><span data-stu-id="74e5c-144">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="74e5c-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="74e5c-145">Response</span></span>

<span data-ttu-id="74e5c-146">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleAssignment](../resources/privilegedroleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74e5c-146">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e5c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="74e5c-147">Example</span></span>
<span data-ttu-id="74e5c-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="74e5c-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="74e5c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="74e5c-149">Request</span></span>
<span data-ttu-id="74e5c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74e5c-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="74e5c-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="74e5c-151">Response</span></span>
<span data-ttu-id="74e5c-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="74e5c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
