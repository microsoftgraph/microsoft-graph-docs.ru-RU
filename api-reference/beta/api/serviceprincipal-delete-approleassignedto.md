---
title: Удаление Аппролеассигнмент, назначенного субъекту службы
description: Удаление Аппролеассигнмент, назначенного субъекту службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: cbb66a092a8d10aed2c063ac82b1ea19ca4dd1b1
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383443"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="f69e5-103">Удаление Аппролеассигнмент, назначенного субъекту службы</span><span class="sxs-lookup"><span data-stu-id="f69e5-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="f69e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f69e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f69e5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f69e5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f69e5-106">Удаляет объект [аппролеассигнмент](../resources/approleassignment.md) , предоставленный субъекту "пользователь", "Группа" или "клиентская служба" для субъекта службы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f69e5-106">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="f69e5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f69e5-107">Permissions</span></span>

<span data-ttu-id="f69e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f69e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f69e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f69e5-110">Permission type</span></span>      | <span data-ttu-id="f69e5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f69e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f69e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f69e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f69e5-113">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="f69e5-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f69e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f69e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f69e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f69e5-115">Not supported.</span></span>    |
|<span data-ttu-id="f69e5-116">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="f69e5-116">Application</span></span> | <span data-ttu-id="f69e5-117">Аппролеассигнмент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f69e5-117">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f69e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f69e5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}
```

> [!NOTE]
> <span data-ttu-id="f69e5-119">Рекомендуется удалять назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектами службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="f69e5-119">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f69e5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f69e5-120">Request headers</span></span>

| <span data-ttu-id="f69e5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f69e5-121">Name</span></span>       | <span data-ttu-id="f69e5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f69e5-122">Type</span></span> | <span data-ttu-id="f69e5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f69e5-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f69e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f69e5-124">Authorization</span></span>  | <span data-ttu-id="f69e5-125">string</span><span class="sxs-lookup"><span data-stu-id="f69e5-125">string</span></span>  | <span data-ttu-id="f69e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f69e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f69e5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f69e5-128">Request body</span></span>

<span data-ttu-id="f69e5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f69e5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f69e5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f69e5-130">Response</span></span>

<span data-ttu-id="f69e5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f69e5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f69e5-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="f69e5-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f69e5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f69e5-134">Request</span></span>

<span data-ttu-id="f69e5-135">Ниже приведен пример запроса на удаление назначения роли приложения от субъекта-службы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f69e5-135">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="f69e5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f69e5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="c"></a>[<span data-ttu-id="f69e5-137">C#</span><span class="sxs-lookup"><span data-stu-id="f69e5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f69e5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f69e5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f69e5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f69e5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f69e5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f69e5-140">Response</span></span>

<span data-ttu-id="f69e5-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f69e5-141">The following is an example of the response.</span></span>

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
