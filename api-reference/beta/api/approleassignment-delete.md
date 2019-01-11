---
title: Удаление appRoleAssignment
description: Удалите appRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 5802ba04cfe8aa5ab12a27bb013d8a36a17096e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814198"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="202ee-103">Удаление appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="202ee-103">Delete appRoleAssignment</span></span>

> <span data-ttu-id="202ee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="202ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="202ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="202ee-106">Удалите appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="202ee-106">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="202ee-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="202ee-107">Permissions</span></span>
<span data-ttu-id="202ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="202ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="202ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="202ee-110">Permission type</span></span>      | <span data-ttu-id="202ee-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="202ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="202ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="202ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="202ee-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="202ee-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="202ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="202ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="202ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202ee-115">Not supported.</span></span>    |
|<span data-ttu-id="202ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="202ee-116">Application</span></span> | <span data-ttu-id="202ee-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202ee-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="202ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="202ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="202ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="202ee-119">Request headers</span></span>
| <span data-ttu-id="202ee-120">Имя</span><span class="sxs-lookup"><span data-stu-id="202ee-120">Name</span></span>       | <span data-ttu-id="202ee-121">Тип</span><span class="sxs-lookup"><span data-stu-id="202ee-121">Type</span></span> | <span data-ttu-id="202ee-122">Описание</span><span class="sxs-lookup"><span data-stu-id="202ee-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="202ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="202ee-123">Authorization</span></span>  | <span data-ttu-id="202ee-124">string</span><span class="sxs-lookup"><span data-stu-id="202ee-124">string</span></span>  | <span data-ttu-id="202ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="202ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="202ee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="202ee-127">Request body</span></span>
<span data-ttu-id="202ee-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="202ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="202ee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="202ee-129">Response</span></span>

<span data-ttu-id="202ee-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="202ee-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="202ee-132">Пример</span><span class="sxs-lookup"><span data-stu-id="202ee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="202ee-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="202ee-133">Request</span></span>
<span data-ttu-id="202ee-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="202ee-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="202ee-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="202ee-135">Response</span></span>
<span data-ttu-id="202ee-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="202ee-136">Here is an example of the response.</span></span> 
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
