---
title: Удаление Аппролеассигнмент, назначенных пользователю
description: Удаление Аппролеассигнмент, предоставленных пользователю.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bdb185bcbb66236ed25f779155c136f2f85e5a26
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290527"
---
# <a name="delete-an-approleassignment-granted-to-a-user"></a><span data-ttu-id="fa927-103">Удаление Аппролеассигнмент, назначенных пользователю</span><span class="sxs-lookup"><span data-stu-id="fa927-103">Delete an appRoleAssignment granted to a user</span></span>

<span data-ttu-id="fa927-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa927-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa927-105">Удаление [аппролеассигнмент](../resources/approleassignment.md) , предоставленных пользователю.</span><span class="sxs-lookup"><span data-stu-id="fa927-105">Delete an [appRoleAssignment](../resources/approleassignment.md) that has been granted to a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa927-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa927-106">Permissions</span></span>

<span data-ttu-id="fa927-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa927-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa927-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa927-109">Permission type</span></span>      | <span data-ttu-id="fa927-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa927-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa927-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa927-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fa927-112">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="fa927-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa927-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa927-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa927-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa927-114">Not supported.</span></span>    |
|<span data-ttu-id="fa927-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa927-115">Application</span></span> | <span data-ttu-id="fa927-116">Аппролеассигнмент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fa927-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa927-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa927-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /users/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="fa927-118">Рекомендуется удалять назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектами службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="fa927-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa927-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa927-119">Request headers</span></span>

| <span data-ttu-id="fa927-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fa927-120">Name</span></span>       | <span data-ttu-id="fa927-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fa927-121">Type</span></span> | <span data-ttu-id="fa927-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fa927-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fa927-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa927-123">Authorization</span></span>  | <span data-ttu-id="fa927-124">string</span><span class="sxs-lookup"><span data-stu-id="fa927-124">string</span></span>  | <span data-ttu-id="fa927-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa927-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa927-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa927-127">Request body</span></span>

<span data-ttu-id="fa927-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa927-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa927-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa927-129">Response</span></span>

<span data-ttu-id="fa927-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa927-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa927-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa927-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa927-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa927-133">Request</span></span>

<span data-ttu-id="fa927-134">Ниже приведен пример запроса на удаление назначения роли приложения.</span><span class="sxs-lookup"><span data-stu-id="fa927-134">Here is an example of the request to delete an app role assignment.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/appRoleAssignments/{id}
```

### <a name="response"></a><span data-ttu-id="fa927-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa927-135">Response</span></span>

<span data-ttu-id="fa927-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa927-136">Here is an example of the response.</span></span>

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
