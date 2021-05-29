---
title: Удаление appRoleAssignment, предоставленного для директора службы
description: Удаление appRoleAssignment, предоставленного для директора службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 35dc83e39fd143b7665e21c98f8ebf638f0a33a1
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703568"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="08269-103">Удаление appRoleAssignment, предоставленного для директора службы</span><span class="sxs-lookup"><span data-stu-id="08269-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="08269-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08269-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="08269-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08269-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08269-106">Удаляет [appRoleAssignment](../resources/approleassignment.md) о том, что директору службы ресурсов, группе или директору клиентской службы предоставлено приложение appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="08269-106">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="08269-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08269-107">Permissions</span></span>

<span data-ttu-id="08269-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08269-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08269-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08269-110">Permission type</span></span>      | <span data-ttu-id="08269-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08269-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08269-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08269-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08269-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08269-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08269-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08269-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08269-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08269-115">Not supported.</span></span>    |
|<span data-ttu-id="08269-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08269-116">Application</span></span> | <span data-ttu-id="08269-117">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08269-117">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08269-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08269-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{principal-id}
```

> [!NOTE]
> <span data-ttu-id="08269-119">В качестве наилучшей практики рекомендуется удалять назначения ролей приложений с помощью отношений директора службы ресурсов, а не отношений назначенного пользователя, группы или директора `appRoleAssignedTo`  `appRoleAssignments` службы.</span><span class="sxs-lookup"><span data-stu-id="08269-119">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08269-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08269-120">Request headers</span></span>

| <span data-ttu-id="08269-121">Имя</span><span class="sxs-lookup"><span data-stu-id="08269-121">Name</span></span>       | <span data-ttu-id="08269-122">Тип</span><span class="sxs-lookup"><span data-stu-id="08269-122">Type</span></span> | <span data-ttu-id="08269-123">Описание</span><span class="sxs-lookup"><span data-stu-id="08269-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08269-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="08269-124">Authorization</span></span>  | <span data-ttu-id="08269-125">string</span><span class="sxs-lookup"><span data-stu-id="08269-125">string</span></span>  | <span data-ttu-id="08269-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08269-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08269-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08269-128">Request body</span></span>

<span data-ttu-id="08269-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08269-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08269-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="08269-130">Response</span></span>

<span data-ttu-id="08269-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="08269-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08269-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="08269-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="08269-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="08269-134">Request</span></span>

<span data-ttu-id="08269-135">Вот пример запроса на удаление назначения роли приложения из основного ресурса службы.</span><span class="sxs-lookup"><span data-stu-id="08269-135">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{principal-id}
```

<span data-ttu-id="08269-136">В этом примере будет id основного средства службы ресурсов и будет id назначенного пользователя, группы или `{resource-SP-id}` `{principalId}` директора клиентской службы.</span><span class="sxs-lookup"><span data-stu-id="08269-136">In this example, `{resource-SP-id}` would be the id of the resource service principal, and `{principalId}` would be the id of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="08269-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="08269-137">Response</span></span>

<span data-ttu-id="08269-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="08269-138">The following is an example of the response.</span></span>

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



