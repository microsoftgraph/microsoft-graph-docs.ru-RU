---
title: Удаление appRoleAssignment, предоставленного для директора службы
description: Удаление appRoleAssignment, предоставленного для директора службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 9fffd71577727eb552b9b18924fde95ef382afb3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441138"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="272a0-103">Удаление appRoleAssignment, предоставленного для директора службы</span><span class="sxs-lookup"><span data-stu-id="272a0-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="272a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="272a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="272a0-105">Удаляет [appRoleAssignment](../resources/approleassignment.md) о том, что директору службы ресурсов, группе или директору клиентской службы предоставлено приложение appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="272a0-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="272a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="272a0-106">Permissions</span></span>

<span data-ttu-id="272a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="272a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="272a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="272a0-109">Permission type</span></span>      | <span data-ttu-id="272a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="272a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="272a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="272a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="272a0-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="272a0-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="272a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="272a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="272a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="272a0-114">Not supported.</span></span>    |
|<span data-ttu-id="272a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="272a0-115">Application</span></span> | <span data-ttu-id="272a0-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="272a0-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="272a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="272a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}
```

> [!NOTE]
> <span data-ttu-id="272a0-118">В качестве наилучшей практики рекомендуется удалять назначения ролей приложений с помощью отношений директора службы ресурсов, а не отношений назначенного пользователя, группы или директора `appRoleAssignedTo`  `appRoleAssignments` службы.</span><span class="sxs-lookup"><span data-stu-id="272a0-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="272a0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="272a0-119">Request headers</span></span>

| <span data-ttu-id="272a0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="272a0-120">Name</span></span>       | <span data-ttu-id="272a0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="272a0-121">Type</span></span> | <span data-ttu-id="272a0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="272a0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="272a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="272a0-123">Authorization</span></span>  | <span data-ttu-id="272a0-124">string</span><span class="sxs-lookup"><span data-stu-id="272a0-124">string</span></span>  | <span data-ttu-id="272a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="272a0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="272a0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="272a0-127">Request body</span></span>

<span data-ttu-id="272a0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="272a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="272a0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="272a0-129">Response</span></span>

<span data-ttu-id="272a0-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="272a0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="272a0-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="272a0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="272a0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="272a0-133">Request</span></span>

<span data-ttu-id="272a0-134">Вот пример запроса на удаление назначения роли приложения из основного ресурса службы.</span><span class="sxs-lookup"><span data-stu-id="272a0-134">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>



# <a name="http"></a>[<span data-ttu-id="272a0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="272a0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}
```
# <a name="c"></a>[<span data-ttu-id="272a0-136">C#</span><span class="sxs-lookup"><span data-stu-id="272a0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="272a0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="272a0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="272a0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="272a0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="272a0-139">Java</span><span class="sxs-lookup"><span data-stu-id="272a0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



<span data-ttu-id="272a0-140">В этом примере является id основного средства службы ресурсов и является id объекта `{resource-SP-id}` appRoleAssignment, представляюшего назначение пользователю, группе или директору клиентской `{appRoleAssignment-id}` службы.</span><span class="sxs-lookup"><span data-stu-id="272a0-140">In this example, `{resource-SP-id}` is the id of the resource service principal, and `{appRoleAssignment-id}` is the id of the appRoleAssignment object that represents an assignment to the user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="272a0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="272a0-141">Response</span></span>

<span data-ttu-id="272a0-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="272a0-142">The following is an example of the response.</span></span>

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

