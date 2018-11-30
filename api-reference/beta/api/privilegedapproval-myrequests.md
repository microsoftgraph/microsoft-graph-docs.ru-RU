---
title: 'privilegedApproval: myRequests'
description: Получите запрашивающего запросов на утверждение.
ms.openlocfilehash: 22485c1ec1127b6c8a3e1f2b40e7d052e885c357
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081277"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="6e555-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="6e555-103">privilegedApproval: myRequests</span></span>

> <span data-ttu-id="6e555-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6e555-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e555-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e555-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e555-106">Получите запрашивающего запросов на утверждение.</span><span class="sxs-lookup"><span data-stu-id="6e555-106">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e555-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e555-107">Permissions</span></span>
<span data-ttu-id="6e555-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e555-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6e555-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e555-110">Permission type</span></span>      | <span data-ttu-id="6e555-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e555-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e555-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e555-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e555-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e555-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e555-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e555-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e555-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e555-115">Not supported.</span></span>    |
|<span data-ttu-id="6e555-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e555-116">Application</span></span> | <span data-ttu-id="6e555-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e555-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e555-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e555-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="6e555-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e555-119">Request headers</span></span>
| <span data-ttu-id="6e555-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6e555-120">Name</span></span>       | <span data-ttu-id="6e555-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6e555-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6e555-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e555-122">Authorization</span></span>  | <span data-ttu-id="6e555-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e555-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e555-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e555-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6e555-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e555-126">Response</span></span>

<span data-ttu-id="6e555-127">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedApproval](../resources/privilegedapproval.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6e555-127">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="6e555-128">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="6e555-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6e555-129">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="6e555-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="6e555-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6e555-130">Example</span></span>
<span data-ttu-id="6e555-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6e555-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e555-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e555-132">Request</span></span>
<span data-ttu-id="6e555-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e555-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="6e555-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e555-134">Response</span></span>
<span data-ttu-id="6e555-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6e555-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
