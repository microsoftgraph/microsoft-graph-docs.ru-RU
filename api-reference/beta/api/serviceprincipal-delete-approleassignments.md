---
title: Удаление Аппролеассигнмент из субъекта службы
description: Удаление Аппролеассигнмент из субъекта службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 1486fdb41db5a5305fc04ec3a508b942658b6194
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333843"
---
# <a name="delete-an-approleassignment-granted-to-a-service-principal"></a><span data-ttu-id="0b600-103">Удаление Аппролеассигнмент, назначенного субъекту службы</span><span class="sxs-lookup"><span data-stu-id="0b600-103">Delete an appRoleAssignment granted to a service principal</span></span>

<span data-ttu-id="0b600-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b600-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b600-105">Удаляет объект [аппролеассигнмент](../resources/approleassignment.md) , предоставленный субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="0b600-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a service principal has been granted.</span></span>

<span data-ttu-id="0b600-106">Роли приложений, назначенные субъектам служб, также называются [разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="0b600-106">App roles which are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="0b600-107">Удаление назначения роли приложения для субъекта-службы эквивалентно отмене предоставления разрешений только для приложения.</span><span class="sxs-lookup"><span data-stu-id="0b600-107">Deleting an app role assignment for a service principal is equivalent to revoking the app-only permission grant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b600-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b600-108">Permissions</span></span>

<span data-ttu-id="0b600-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b600-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b600-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b600-111">Permission type</span></span>      | <span data-ttu-id="0b600-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b600-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b600-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b600-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0b600-114">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0b600-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b600-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b600-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b600-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b600-116">Not supported.</span></span>    |
|<span data-ttu-id="0b600-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b600-117">Application</span></span> | <span data-ttu-id="0b600-118">Аппролеассигнмент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b600-118">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b600-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b600-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="0b600-120">Рекомендуется удалять назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектами службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="0b600-120">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b600-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b600-121">Request headers</span></span>

| <span data-ttu-id="0b600-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0b600-122">Name</span></span>       | <span data-ttu-id="0b600-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0b600-123">Type</span></span> | <span data-ttu-id="0b600-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0b600-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b600-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b600-125">Authorization</span></span>  | <span data-ttu-id="0b600-126">string</span><span class="sxs-lookup"><span data-stu-id="0b600-126">string</span></span>  | <span data-ttu-id="0b600-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b600-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b600-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b600-129">Request body</span></span>

<span data-ttu-id="0b600-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b600-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b600-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b600-131">Response</span></span>

<span data-ttu-id="0b600-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0b600-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b600-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b600-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b600-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b600-135">Request</span></span>

<span data-ttu-id="0b600-136">Ниже приведен пример запроса на удаление назначения роли приложения.</span><span class="sxs-lookup"><span data-stu-id="0b600-136">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b600-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b600-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="0b600-138">C#</span><span class="sxs-lookup"><span data-stu-id="0b600-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b600-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b600-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b600-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b600-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b600-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b600-141">Response</span></span>

<span data-ttu-id="0b600-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0b600-142">The following is an example of the response.</span></span>

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
