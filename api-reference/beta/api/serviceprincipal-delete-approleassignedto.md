---
title: Удаление Аппролеассигнмент, назначенного субъекту службы
description: Удаление Аппролеассигнмент, назначенного субъекту службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: dc7910b4e76ba177ca5c63103faab6890b8d4489
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970815"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="dcf03-103">Удаление Аппролеассигнмент, назначенного субъекту службы</span><span class="sxs-lookup"><span data-stu-id="dcf03-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="dcf03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcf03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dcf03-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcf03-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf03-106">Удаляет объект [аппролеассигнмент](../resources/approleassignment.md) , предоставленный субъекту "пользователь", "Группа" или "клиентская служба" для субъекта службы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dcf03-106">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf03-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcf03-107">Permissions</span></span>

<span data-ttu-id="dcf03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcf03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcf03-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcf03-110">Permission type</span></span>      | <span data-ttu-id="dcf03-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcf03-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcf03-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcf03-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dcf03-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dcf03-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dcf03-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcf03-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcf03-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcf03-115">Not supported.</span></span>    |
|<span data-ttu-id="dcf03-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcf03-116">Application</span></span> | <span data-ttu-id="dcf03-117">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcf03-117">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcf03-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcf03-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}
```

> [!NOTE]
> <span data-ttu-id="dcf03-119">Рекомендуется удалять назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектами службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="dcf03-119">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcf03-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcf03-120">Request headers</span></span>

| <span data-ttu-id="dcf03-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dcf03-121">Name</span></span>       | <span data-ttu-id="dcf03-122">Тип</span><span class="sxs-lookup"><span data-stu-id="dcf03-122">Type</span></span> | <span data-ttu-id="dcf03-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dcf03-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dcf03-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcf03-124">Authorization</span></span>  | <span data-ttu-id="dcf03-125">string</span><span class="sxs-lookup"><span data-stu-id="dcf03-125">string</span></span>  | <span data-ttu-id="dcf03-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcf03-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcf03-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dcf03-128">Request body</span></span>

<span data-ttu-id="dcf03-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dcf03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf03-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcf03-130">Response</span></span>

<span data-ttu-id="dcf03-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dcf03-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcf03-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="dcf03-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcf03-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcf03-134">Request</span></span>

<span data-ttu-id="dcf03-135">Ниже приведен пример запроса на удаление назначения роли приложения от субъекта-службы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dcf03-135">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="dcf03-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf03-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="c"></a>[<span data-ttu-id="dcf03-137">C#</span><span class="sxs-lookup"><span data-stu-id="dcf03-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcf03-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcf03-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcf03-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcf03-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcf03-140">Java</span><span class="sxs-lookup"><span data-stu-id="dcf03-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dcf03-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcf03-141">Response</span></span>

<span data-ttu-id="dcf03-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dcf03-142">The following is an example of the response.</span></span>

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


