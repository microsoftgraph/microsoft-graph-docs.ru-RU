---
title: Удаление Унифиедролеассигнментмултипле
description: Удаление объекта Унифиедролеассигнментмултипле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 18b164b09ad3b06f02b3be0890aeada32946b48b
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160420"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="8e912-103">Удаление Унифиедролеассигнментмултипле</span><span class="sxs-lookup"><span data-stu-id="8e912-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="8e912-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e912-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e912-105">Удаление объекта [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="8e912-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="8e912-106">Это относится к приложению RBAC, которое поддерживает несколько субъектов и областей.</span><span class="sxs-lookup"><span data-stu-id="8e912-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="8e912-107">Microsoft Intune это приложение.</span><span class="sxs-lookup"><span data-stu-id="8e912-107">Microsoft Intune is such an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e912-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e912-108">Permissions</span></span>

<span data-ttu-id="8e912-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e912-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e912-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e912-111">Permission type</span></span> | <span data-ttu-id="8e912-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e912-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="8e912-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e912-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8e912-114">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="8e912-114">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="8e912-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e912-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e912-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e912-116">Not supported.</span></span> |
| <span data-ttu-id="8e912-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e912-117">Application</span></span> | <span data-ttu-id="8e912-118">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="8e912-118">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e912-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e912-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8e912-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e912-120">Request headers</span></span>

| <span data-ttu-id="8e912-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8e912-121">Name</span></span> | <span data-ttu-id="8e912-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8e912-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="8e912-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e912-123">Authorization</span></span> | <span data-ttu-id="8e912-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8e912-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e912-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e912-125">Request body</span></span>

<span data-ttu-id="8e912-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e912-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e912-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e912-127">Response</span></span>

<span data-ttu-id="8e912-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8e912-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e912-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8e912-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e912-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e912-131">Request</span></span>

<span data-ttu-id="8e912-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e912-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```

### <a name="response"></a><span data-ttu-id="8e912-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e912-133">Response</span></span>

<span data-ttu-id="8e912-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e912-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->