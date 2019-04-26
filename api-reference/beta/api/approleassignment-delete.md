---
title: Удаление объекта AppRoleAssignment
description: Удаление Аппролеассигнмент.
localization_priority: Normal
ms.openlocfilehash: 2e1c39078005f2dabaabd9181ff592d0898c9355
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322621"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="b72ae-103">Удаление объекта AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b72ae-103">Delete appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b72ae-104">Удаление Аппролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="b72ae-104">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="b72ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b72ae-105">Permissions</span></span>
<span data-ttu-id="b72ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b72ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b72ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b72ae-108">Permission type</span></span>      | <span data-ttu-id="b72ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b72ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b72ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b72ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b72ae-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b72ae-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b72ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b72ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b72ae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b72ae-113">Not supported.</span></span>    |
|<span data-ttu-id="b72ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b72ae-114">Application</span></span> | <span data-ttu-id="b72ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b72ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b72ae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b72ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b72ae-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b72ae-117">Request headers</span></span>
| <span data-ttu-id="b72ae-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b72ae-118">Name</span></span>       | <span data-ttu-id="b72ae-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b72ae-119">Type</span></span> | <span data-ttu-id="b72ae-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b72ae-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b72ae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b72ae-121">Authorization</span></span>  | <span data-ttu-id="b72ae-122">string</span><span class="sxs-lookup"><span data-stu-id="b72ae-122">string</span></span>  | <span data-ttu-id="b72ae-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b72ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b72ae-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b72ae-125">Request body</span></span>
<span data-ttu-id="b72ae-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b72ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b72ae-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b72ae-127">Response</span></span>

<span data-ttu-id="b72ae-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b72ae-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b72ae-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b72ae-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b72ae-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b72ae-131">Request</span></span>
<span data-ttu-id="b72ae-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b72ae-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="b72ae-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b72ae-133">Response</span></span>
<span data-ttu-id="b72ae-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b72ae-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
