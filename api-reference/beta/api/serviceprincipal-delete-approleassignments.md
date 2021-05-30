---
title: Удаление appRoleAssignment из основной службы
description: Удаление appRoleAssignment из основной службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 8e4f2c986723c8dab08eab88b6b80f5f72d6f76c
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703582"
---
# <a name="delete-an-approleassignment-granted-to-a-service-principal"></a><span data-ttu-id="776fd-103">Удаление appRoleAssignment, предоставленного директору службы</span><span class="sxs-lookup"><span data-stu-id="776fd-103">Delete an appRoleAssignment granted to a service principal</span></span>

<span data-ttu-id="776fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="776fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="776fd-105">Удаляет [приложение AppRoleAssignment,](../resources/approleassignment.md) предоставленное директору службы.</span><span class="sxs-lookup"><span data-stu-id="776fd-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a service principal has been granted.</span></span>

<span data-ttu-id="776fd-106">Роли приложений, которые назначены директорам служб, также называются [разрешениями приложений.](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)</span><span class="sxs-lookup"><span data-stu-id="776fd-106">App roles which are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="776fd-107">Удаление назначения роли приложения для директора службы эквивалентно отмене разрешения только для приложения.</span><span class="sxs-lookup"><span data-stu-id="776fd-107">Deleting an app role assignment for a service principal is equivalent to revoking the app-only permission grant.</span></span>

## <a name="permissions"></a><span data-ttu-id="776fd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="776fd-108">Permissions</span></span>

<span data-ttu-id="776fd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="776fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="776fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="776fd-111">Permission type</span></span>      | <span data-ttu-id="776fd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="776fd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="776fd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="776fd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="776fd-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="776fd-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="776fd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="776fd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="776fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="776fd-116">Not supported.</span></span>    |
|<span data-ttu-id="776fd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="776fd-117">Application</span></span> | <span data-ttu-id="776fd-118">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="776fd-118">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="776fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="776fd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}
```

> [!NOTE]
> <span data-ttu-id="776fd-120">В качестве наилучшей практики рекомендуется удалять назначения ролей приложений с помощью отношений директора службы ресурсов, а не отношений назначенного пользователя, группы или директора `appRoleAssignedTo`  `appRoleAssignments` службы.</span><span class="sxs-lookup"><span data-stu-id="776fd-120">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="776fd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="776fd-121">Request headers</span></span>

| <span data-ttu-id="776fd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="776fd-122">Name</span></span>       | <span data-ttu-id="776fd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="776fd-123">Type</span></span> | <span data-ttu-id="776fd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="776fd-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="776fd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="776fd-125">Authorization</span></span>  | <span data-ttu-id="776fd-126">string</span><span class="sxs-lookup"><span data-stu-id="776fd-126">string</span></span>  | <span data-ttu-id="776fd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="776fd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="776fd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="776fd-129">Request body</span></span>

<span data-ttu-id="776fd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="776fd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="776fd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="776fd-131">Response</span></span>

<span data-ttu-id="776fd-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="776fd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="776fd-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="776fd-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="776fd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="776fd-135">Request</span></span>

<span data-ttu-id="776fd-136">Вот пример запроса на удаление назначения роли приложения.</span><span class="sxs-lookup"><span data-stu-id="776fd-136">Here is an example of the request to delete an app role assignment.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}
```

### <a name="response"></a><span data-ttu-id="776fd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="776fd-137">Response</span></span>

<span data-ttu-id="776fd-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="776fd-138">The following is an example of the response.</span></span>

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
