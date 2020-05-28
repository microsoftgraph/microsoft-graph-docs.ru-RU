---
title: Удаление Аппролеассигнмент из группы
description: Удаление Аппролеассигнмент, предоставленных группе.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 3e4c0b7764cefffc5f25689c84a960ec72eca733
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383849"
---
# <a name="delete-an-approleassignment-granted-to-a-group"></a><span data-ttu-id="ecb79-103">Удаление Аппролеассигнмент, назначенного группе</span><span class="sxs-lookup"><span data-stu-id="ecb79-103">Delete an appRoleAssignment granted to a group</span></span>

<span data-ttu-id="ecb79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecb79-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecb79-105">Удаляет объект [аппролеассигнмент](../resources/approleassignment.md) , предоставленный группе.</span><span class="sxs-lookup"><span data-stu-id="ecb79-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) which a group has been granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="ecb79-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ecb79-106">Permissions</span></span>

<span data-ttu-id="ecb79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecb79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecb79-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecb79-109">Permission type</span></span>      | <span data-ttu-id="ecb79-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecb79-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ecb79-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecb79-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ecb79-112">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ecb79-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ecb79-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecb79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ecb79-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecb79-114">Not supported.</span></span>    |
|<span data-ttu-id="ecb79-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="ecb79-115">Application</span></span> | <span data-ttu-id="ecb79-116">Аппролеассигнмент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ecb79-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ecb79-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecb79-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="ecb79-118">Рекомендуется удалять назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектами службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="ecb79-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ecb79-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecb79-119">Request headers</span></span>

| <span data-ttu-id="ecb79-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ecb79-120">Name</span></span>       | <span data-ttu-id="ecb79-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ecb79-121">Type</span></span> | <span data-ttu-id="ecb79-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ecb79-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ecb79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecb79-123">Authorization</span></span>  | <span data-ttu-id="ecb79-124">string</span><span class="sxs-lookup"><span data-stu-id="ecb79-124">string</span></span>  | <span data-ttu-id="ecb79-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecb79-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecb79-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ecb79-127">Request body</span></span>

<span data-ttu-id="ecb79-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ecb79-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecb79-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecb79-129">Response</span></span>

<span data-ttu-id="ecb79-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ecb79-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ecb79-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ecb79-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ecb79-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecb79-133">Request</span></span>

<span data-ttu-id="ecb79-134">Ниже приведен пример запроса на удаление назначения роли приложения.</span><span class="sxs-lookup"><span data-stu-id="ecb79-134">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="ecb79-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ecb79-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="ecb79-136">C#</span><span class="sxs-lookup"><span data-stu-id="ecb79-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ecb79-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ecb79-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ecb79-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ecb79-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ecb79-139">Java</span><span class="sxs-lookup"><span data-stu-id="ecb79-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ecb79-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecb79-140">Response</span></span>

<span data-ttu-id="ecb79-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ecb79-141">The following is an example of the response.</span></span>

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
