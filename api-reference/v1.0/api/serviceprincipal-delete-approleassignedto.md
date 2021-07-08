---
title: Удаление appRoleAssignment, предоставленного для директора службы
description: Удаление appRoleAssignment, предоставленного для директора службы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f1d874ee77733d81da3a94f448f57675c15062bc
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317044"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="36fe7-103">Удаление appRoleAssignment, предоставленного для директора службы</span><span class="sxs-lookup"><span data-stu-id="36fe7-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="36fe7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36fe7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36fe7-105">Удаляет [appRoleAssignment](../resources/approleassignment.md) о том, что директору службы ресурсов, группе или директору клиентской службы предоставлено приложение appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="36fe7-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="36fe7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36fe7-106">Permissions</span></span>

<span data-ttu-id="36fe7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36fe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36fe7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36fe7-109">Permission type</span></span>      | <span data-ttu-id="36fe7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36fe7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36fe7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36fe7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36fe7-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36fe7-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36fe7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36fe7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36fe7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36fe7-114">Not supported.</span></span>    |
|<span data-ttu-id="36fe7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36fe7-115">Application</span></span> | <span data-ttu-id="36fe7-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36fe7-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36fe7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36fe7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}
```

> [!NOTE]
> <span data-ttu-id="36fe7-118">В качестве наилучшей практики рекомендуется удалять назначения ролей приложений с помощью отношений директора службы ресурсов, а не отношений назначенного пользователя, группы или директора `appRoleAssignedTo`  `appRoleAssignments` службы.</span><span class="sxs-lookup"><span data-stu-id="36fe7-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36fe7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36fe7-119">Request headers</span></span>

| <span data-ttu-id="36fe7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="36fe7-120">Name</span></span>       | <span data-ttu-id="36fe7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="36fe7-121">Type</span></span> | <span data-ttu-id="36fe7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="36fe7-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="36fe7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36fe7-123">Authorization</span></span>  | <span data-ttu-id="36fe7-124">string</span><span class="sxs-lookup"><span data-stu-id="36fe7-124">string</span></span>  | <span data-ttu-id="36fe7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36fe7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36fe7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36fe7-127">Request body</span></span>

<span data-ttu-id="36fe7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36fe7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36fe7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="36fe7-129">Response</span></span>

<span data-ttu-id="36fe7-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="36fe7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36fe7-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="36fe7-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36fe7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="36fe7-133">Request</span></span>

<span data-ttu-id="36fe7-134">Вот пример запроса на удаление назначения роли приложения из основного ресурса службы.</span><span class="sxs-lookup"><span data-stu-id="36fe7-134">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>


<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}
```


<span data-ttu-id="36fe7-135">В этом примере является id основного средства службы ресурсов и является id объекта `{resource-SP-id}` appRoleAssignment, представляюшего назначение пользователю, группе или директору клиентской `{appRoleAssignment-id}` службы.</span><span class="sxs-lookup"><span data-stu-id="36fe7-135">In this example, `{resource-SP-id}` is the id of the resource service principal, and `{appRoleAssignment-id}` is the id of the appRoleAssignment object that represents an assignment to the user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="36fe7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="36fe7-136">Response</span></span>

<span data-ttu-id="36fe7-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36fe7-137">The following is an example of the response.</span></span>

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

