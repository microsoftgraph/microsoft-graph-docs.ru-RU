---
title: Удаление appRoleAssignment, предоставленного для директора службы
description: Удаление appRoleAssignment, предоставленного для директора службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: bd66bed87d46f548a0c2f9ee76cfe0cd761db1fa
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703617"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="77b9c-103">Удаление appRoleAssignment, предоставленного для директора службы</span><span class="sxs-lookup"><span data-stu-id="77b9c-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="77b9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77b9c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77b9c-105">Удаляет [appRoleAssignment](../resources/approleassignment.md) о том, что директору службы ресурсов, группе или директору клиентской службы предоставлено приложение appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="77b9c-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="77b9c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77b9c-106">Permissions</span></span>

<span data-ttu-id="77b9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77b9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77b9c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77b9c-109">Permission type</span></span>      | <span data-ttu-id="77b9c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77b9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77b9c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77b9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77b9c-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77b9c-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77b9c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77b9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77b9c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77b9c-114">Not supported.</span></span>    |
|<span data-ttu-id="77b9c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77b9c-115">Application</span></span> | <span data-ttu-id="77b9c-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77b9c-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77b9c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77b9c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{principal-id}
```

> [!NOTE]
> <span data-ttu-id="77b9c-118">В качестве наилучшей практики рекомендуется удалять назначения ролей приложений с помощью отношений директора службы ресурсов, а не отношений назначенного пользователя, группы или директора `appRoleAssignedTo`  `appRoleAssignments` службы.</span><span class="sxs-lookup"><span data-stu-id="77b9c-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77b9c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77b9c-119">Request headers</span></span>

| <span data-ttu-id="77b9c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="77b9c-120">Name</span></span>       | <span data-ttu-id="77b9c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="77b9c-121">Type</span></span> | <span data-ttu-id="77b9c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="77b9c-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="77b9c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77b9c-123">Authorization</span></span>  | <span data-ttu-id="77b9c-124">string</span><span class="sxs-lookup"><span data-stu-id="77b9c-124">string</span></span>  | <span data-ttu-id="77b9c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77b9c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77b9c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77b9c-127">Request body</span></span>

<span data-ttu-id="77b9c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77b9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77b9c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="77b9c-129">Response</span></span>

<span data-ttu-id="77b9c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="77b9c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77b9c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="77b9c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77b9c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="77b9c-133">Request</span></span>

<span data-ttu-id="77b9c-134">Вот пример запроса на удаление назначения роли приложения из основного ресурса службы.</span><span class="sxs-lookup"><span data-stu-id="77b9c-134">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{principalId}
```

<span data-ttu-id="77b9c-135">В этом примере будет id основного средства службы ресурсов и будет id назначенного пользователя, группы или `{resource-SP-id}` `{principalId}` директора клиентской службы.</span><span class="sxs-lookup"><span data-stu-id="77b9c-135">In this example, `{resource-SP-id}` would be the id of the resource service principal, and `{principalId}` would be the id of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="77b9c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="77b9c-136">Response</span></span>

<span data-ttu-id="77b9c-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="77b9c-137">The following is an example of the response.</span></span>

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

