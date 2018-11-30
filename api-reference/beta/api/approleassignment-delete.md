---
title: Удаление appRoleAssignment
description: Удалите appRoleAssignment.
ms.openlocfilehash: 1673f3f04d03154242497682da3fcbdaf4248412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076329"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="8d3d5-103">Удаление appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8d3d5-103">Delete appRoleAssignment</span></span>

> <span data-ttu-id="8d3d5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d3d5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d3d5-106">Удалите appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-106">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d3d5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d3d5-107">Permissions</span></span>
<span data-ttu-id="8d3d5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d3d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d3d5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d3d5-110">Permission type</span></span>      | <span data-ttu-id="8d3d5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d3d5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d3d5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d3d5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d3d5-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d3d5-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d3d5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d3d5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d3d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-115">Not supported.</span></span>    |
|<span data-ttu-id="8d3d5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d3d5-116">Application</span></span> | <span data-ttu-id="8d3d5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d3d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d3d5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8d3d5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d3d5-119">Request headers</span></span>
| <span data-ttu-id="8d3d5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8d3d5-120">Name</span></span>       | <span data-ttu-id="8d3d5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8d3d5-121">Type</span></span> | <span data-ttu-id="8d3d5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8d3d5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8d3d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d3d5-123">Authorization</span></span>  | <span data-ttu-id="8d3d5-124">string</span><span class="sxs-lookup"><span data-stu-id="8d3d5-124">string</span></span>  | <span data-ttu-id="8d3d5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d3d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d3d5-127">Request body</span></span>
<span data-ttu-id="8d3d5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d3d5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3d5-129">Response</span></span>

<span data-ttu-id="8d3d5-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d3d5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8d3d5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d3d5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d3d5-133">Request</span></span>
<span data-ttu-id="8d3d5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="8d3d5-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d3d5-135">Response</span></span>
<span data-ttu-id="8d3d5-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d3d5-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->