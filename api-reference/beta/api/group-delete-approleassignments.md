---
title: Удаление Аппролеассигнмент из группы
description: Удаление Аппролеассигнмент, предоставленных группе.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8fe9999c1e7953df537054d382d30228c4f81d94
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289462"
---
# <a name="delete-an-approleassignment-granted-to-a-group"></a><span data-ttu-id="2ba24-103">Удаление Аппролеассигнмент, назначенного группе</span><span class="sxs-lookup"><span data-stu-id="2ba24-103">Delete an appRoleAssignment granted to a group</span></span>

<span data-ttu-id="2ba24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ba24-105">Удаляет объект [аппролеассигнмент](../resources/approleassignment.md) , предоставленный группе.</span><span class="sxs-lookup"><span data-stu-id="2ba24-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a group has been granted.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ba24-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ba24-106">Permissions</span></span>

<span data-ttu-id="2ba24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ba24-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ba24-109">Permission type</span></span>      | <span data-ttu-id="2ba24-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ba24-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ba24-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ba24-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ba24-112">Аппролеассигнмент. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="2ba24-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ba24-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ba24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ba24-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ba24-114">Not supported.</span></span>    |
|<span data-ttu-id="2ba24-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ba24-115">Application</span></span> | <span data-ttu-id="2ba24-116">Аппролеассигнмент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2ba24-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ba24-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ba24-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /groups/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="2ba24-118">Рекомендуется удалять назначения ролей приложений с помощью `appRoleAssignedTo` отношения между субъектами службы _ресурсов_ , а не с `appRoleAssignments` назначенным пользователем, группой или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="2ba24-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ba24-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ba24-119">Request headers</span></span>

| <span data-ttu-id="2ba24-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2ba24-120">Name</span></span>       | <span data-ttu-id="2ba24-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2ba24-121">Type</span></span> | <span data-ttu-id="2ba24-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba24-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2ba24-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ba24-123">Authorization</span></span>  | <span data-ttu-id="2ba24-124">string</span><span class="sxs-lookup"><span data-stu-id="2ba24-124">string</span></span>  | <span data-ttu-id="2ba24-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ba24-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ba24-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ba24-127">Request body</span></span>

<span data-ttu-id="2ba24-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ba24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ba24-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba24-129">Response</span></span>

<span data-ttu-id="2ba24-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2ba24-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ba24-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ba24-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ba24-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ba24-133">Request</span></span>

<span data-ttu-id="2ba24-134">Ниже приведен пример запроса на удаление назначения роли приложения.</span><span class="sxs-lookup"><span data-stu-id="2ba24-134">Here is an example of the request to delete an app role assignment.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/groups/{id}/appRoleAssignments/{id}
```

### <a name="response"></a><span data-ttu-id="2ba24-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ba24-135">Response</span></span>

<span data-ttu-id="2ba24-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ba24-136">The following is an example of the response.</span></span>

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
