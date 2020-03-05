---
title: Создание Унифиедролеассигнмент
description: Создание нового объекта Унифиедролеассигнмент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 672eac457659c3af05f0a3e1fc92ec0fe283746e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454521"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="922d4-103">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="922d4-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="922d4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="922d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="922d4-105">Создание нового объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="922d4-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="922d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="922d4-106">Permissions</span></span>

<span data-ttu-id="922d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="922d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="922d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="922d4-109">Permission type</span></span>                        | <span data-ttu-id="922d4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="922d4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="922d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="922d4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="922d4-112">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="922d4-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="922d4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="922d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="922d4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="922d4-114">Not supported.</span></span> |
| <span data-ttu-id="922d4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="922d4-115">Application</span></span>                            | <span data-ttu-id="922d4-116">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="922d4-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="922d4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="922d4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="922d4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="922d4-118">Request headers</span></span>

| <span data-ttu-id="922d4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="922d4-119">Name</span></span>          | <span data-ttu-id="922d4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="922d4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="922d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="922d4-121">Authorization</span></span> | <span data-ttu-id="922d4-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="922d4-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="922d4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="922d4-123">Request body</span></span>

<span data-ttu-id="922d4-124">В тексте запроса добавьте представление объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="922d4-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="922d4-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="922d4-125">Response</span></span>

<span data-ttu-id="922d4-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="922d4-126">If successful, this method returns `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="922d4-127">Пример</span><span class="sxs-lookup"><span data-stu-id="922d4-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="922d4-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="922d4-128">Request</span></span>

<span data-ttu-id="922d4-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="922d4-129">The following is an example of the request.</span></span> <span data-ttu-id="922d4-130">Обратите внимание на использование параметра Ролетемплатеид для Роледефинитионид.</span><span class="sxs-lookup"><span data-stu-id="922d4-130">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="922d4-131">Роледефинитионид может быть либо идентификатором шаблона на уровне службы, либо Роледефинитионид, зависящим от каталога.</span><span class="sxs-lookup"><span data-stu-id="922d4-131">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>

# <a name="http"></a>[<span data-ttu-id="922d4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="922d4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{ 
    "principalId":"a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    "roleDefinitionId":"b0f54661-2d74-4c50-afa3-1ec803f12efe",
    "resourceScope":"/"
}
```
# <a name="c"></a>[<span data-ttu-id="922d4-133">C#</span><span class="sxs-lookup"><span data-stu-id="922d4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="922d4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="922d4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="922d4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="922d4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="922d4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="922d4-136">Response</span></span>

<span data-ttu-id="922d4-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="922d4-137">The following is an example of the response.</span></span>

> <span data-ttu-id="922d4-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="922d4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "YUb1sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHVi2I-1",
    "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    "resourceScope": "/",
    "roleDefinitionId": "b0f54661-2d74-4c50-afa3-1ec803f12efe"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
