---
title: Удаление Аппролеассигнмент, назначенных пользователю
description: Удаление Аппролеассигнмент, предоставленных пользователю.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4ad979a7fc053ceea6a593f0b1e215cb04acf737
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383898"
---
# <a name="delete-an-approleassignment-granted-to-a-user"></a><span data-ttu-id="c955d-103">Удаление Аппролеассигнмент, назначенных пользователю</span><span class="sxs-lookup"><span data-stu-id="c955d-103">Delete an appRoleAssignment granted to a user</span></span>

<span data-ttu-id="c955d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c955d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c955d-105">Удаление [аппролеассигнмент](../resources/approleassignment.md) , предоставленных пользователю.</span><span class="sxs-lookup"><span data-stu-id="c955d-105">Delete an [appRoleAssignment](../resources/approleassignment.md) that has been granted to a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c955d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c955d-106">Permissions</span></span>

<span data-ttu-id="c955d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c955d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c955d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c955d-109">Permission type</span></span>      | <span data-ttu-id="c955d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c955d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c955d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c955d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c955d-112">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c955d-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c955d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c955d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c955d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c955d-114">Not supported.</span></span>    |
|<span data-ttu-id="c955d-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="c955d-115">Application</span></span> | <span data-ttu-id="c955d-116">Аппролеассигнмент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c955d-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c955d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c955d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /users/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="c955d-118">Рекомендуется удалять назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектами службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="c955d-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c955d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c955d-119">Request headers</span></span>

| <span data-ttu-id="c955d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c955d-120">Name</span></span>       | <span data-ttu-id="c955d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c955d-121">Type</span></span> | <span data-ttu-id="c955d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c955d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c955d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c955d-123">Authorization</span></span>  | <span data-ttu-id="c955d-124">string</span><span class="sxs-lookup"><span data-stu-id="c955d-124">string</span></span>  | <span data-ttu-id="c955d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c955d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c955d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c955d-127">Request body</span></span>

<span data-ttu-id="c955d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c955d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c955d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c955d-129">Response</span></span>

<span data-ttu-id="c955d-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c955d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c955d-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="c955d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c955d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c955d-133">Request</span></span>

<span data-ttu-id="c955d-134">Ниже приведен пример запроса на удаление назначения роли приложения.</span><span class="sxs-lookup"><span data-stu-id="c955d-134">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="c955d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c955d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="c955d-136">C#</span><span class="sxs-lookup"><span data-stu-id="c955d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c955d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c955d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c955d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c955d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c955d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c955d-139">Response</span></span>

<span data-ttu-id="c955d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c955d-140">Here is an example of the response.</span></span>

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
  "suppressions": [
  ]
}
-->
