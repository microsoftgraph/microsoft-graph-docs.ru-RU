---
title: Создание Унифиедролеассигнмент
description: Создание нового объекта Унифиедролеассигнмент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 42a747377ab8e5ae21c87b0fe529e92028d1a013
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461302"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="b9b27-103">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="b9b27-103">Create unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9b27-104">Создание нового объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b9b27-104">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9b27-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9b27-105">Permissions</span></span>

<span data-ttu-id="b9b27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9b27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9b27-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9b27-108">Permission type</span></span>                        | <span data-ttu-id="b9b27-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9b27-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9b27-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9b27-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9b27-111">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="b9b27-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="b9b27-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9b27-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9b27-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9b27-113">Not supported.</span></span> |
| <span data-ttu-id="b9b27-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9b27-114">Application</span></span>                            | <span data-ttu-id="b9b27-115">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="b9b27-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9b27-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9b27-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b9b27-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9b27-117">Request headers</span></span>

| <span data-ttu-id="b9b27-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b9b27-118">Name</span></span>          | <span data-ttu-id="b9b27-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b9b27-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b9b27-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9b27-120">Authorization</span></span> | <span data-ttu-id="b9b27-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b9b27-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9b27-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9b27-122">Request body</span></span>

<span data-ttu-id="b9b27-123">В тексте запроса добавьте представление объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9b27-123">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b9b27-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9b27-124">Response</span></span>

<span data-ttu-id="b9b27-125">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9b27-125">If successful, this method returns `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9b27-126">Пример</span><span class="sxs-lookup"><span data-stu-id="b9b27-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9b27-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9b27-127">Request</span></span>

<span data-ttu-id="b9b27-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9b27-128">The following is an example of the request.</span></span> <span data-ttu-id="b9b27-129">Обратите внимание на использование параметра Ролетемплатеид для Роледефинитионид.</span><span class="sxs-lookup"><span data-stu-id="b9b27-129">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="b9b27-130">Роледефинитионид может быть либо идентификатором шаблона на уровне службы, либо Роледефинитионид, зависящим от каталога.</span><span class="sxs-lookup"><span data-stu-id="b9b27-130">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b9b27-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9b27-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b9b27-132">C#</span><span class="sxs-lookup"><span data-stu-id="b9b27-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9b27-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9b27-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b9b27-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b9b27-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9b27-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9b27-135">Response</span></span>

<span data-ttu-id="b9b27-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9b27-136">The following is an example of the response.</span></span>

> <span data-ttu-id="b9b27-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9b27-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
