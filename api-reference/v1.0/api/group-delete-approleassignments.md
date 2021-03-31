---
title: Удаление appRoleAssignment из группы
description: Удаление appRoleAssignment, предоставленного группе.
localization_priority: Normal
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: b1d8898da9b71474d298de5f76b17000f7ef7b8b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469418"
---
# <a name="delete-an-approleassignment-granted-to-a-group"></a><span data-ttu-id="eab34-103">Удаление appRoleAssignment, предоставленного группе</span><span class="sxs-lookup"><span data-stu-id="eab34-103">Delete an appRoleAssignment granted to a group</span></span>

<span data-ttu-id="eab34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eab34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eab34-105">Удаляет [appRoleAssignment,](../resources/approleassignment.md) предоставленную группе.</span><span class="sxs-lookup"><span data-stu-id="eab34-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a group has been granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="eab34-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eab34-106">Permissions</span></span>

<span data-ttu-id="eab34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eab34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eab34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eab34-109">Permission type</span></span>      | <span data-ttu-id="eab34-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eab34-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eab34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eab34-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eab34-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eab34-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eab34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eab34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eab34-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eab34-114">Not supported.</span></span>    |
|<span data-ttu-id="eab34-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eab34-115">Application</span></span> | <span data-ttu-id="eab34-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eab34-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eab34-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eab34-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="eab34-118">В качестве наилучшей практики рекомендуется удалять назначения ролей приложений с помощью отношений директора службы ресурсов, а не отношений назначенного пользователя, группы или директора `appRoleAssignedTo`  `appRoleAssignments` службы.</span><span class="sxs-lookup"><span data-stu-id="eab34-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eab34-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eab34-119">Request headers</span></span>

| <span data-ttu-id="eab34-120">Имя</span><span class="sxs-lookup"><span data-stu-id="eab34-120">Name</span></span>       | <span data-ttu-id="eab34-121">Тип</span><span class="sxs-lookup"><span data-stu-id="eab34-121">Type</span></span> | <span data-ttu-id="eab34-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eab34-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eab34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eab34-123">Authorization</span></span>  | <span data-ttu-id="eab34-124">string</span><span class="sxs-lookup"><span data-stu-id="eab34-124">string</span></span>  | <span data-ttu-id="eab34-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eab34-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eab34-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eab34-127">Request body</span></span>

<span data-ttu-id="eab34-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eab34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eab34-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab34-129">Response</span></span>

<span data-ttu-id="eab34-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="eab34-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eab34-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="eab34-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eab34-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eab34-133">Request</span></span>

<span data-ttu-id="eab34-134">Вот пример запроса на удаление назначения роли приложения.</span><span class="sxs-lookup"><span data-stu-id="eab34-134">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="eab34-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eab34-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="eab34-136">C#</span><span class="sxs-lookup"><span data-stu-id="eab34-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eab34-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eab34-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eab34-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eab34-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eab34-139">Java</span><span class="sxs-lookup"><span data-stu-id="eab34-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eab34-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab34-140">Response</span></span>

<span data-ttu-id="eab34-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="eab34-141">The following is an example of the response.</span></span>

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

