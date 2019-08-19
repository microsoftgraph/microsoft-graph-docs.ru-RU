---
title: Создание Унифиедроледефинитион
description: Создание нового объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74a67f090d37fe6eff0b4910862eabafcfcd27c7
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461286"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="673f2-103">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="673f2-103">Create unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="673f2-104">Создание нового объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="673f2-104">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="673f2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="673f2-105">Permissions</span></span>

<span data-ttu-id="673f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="673f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="673f2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="673f2-108">Permission type</span></span>                        | <span data-ttu-id="673f2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="673f2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="673f2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="673f2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="673f2-111">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="673f2-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="673f2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="673f2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="673f2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="673f2-113">Not supported.</span></span> |
| <span data-ttu-id="673f2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="673f2-114">Application</span></span>                            | <span data-ttu-id="673f2-115">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="673f2-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="673f2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="673f2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="673f2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="673f2-117">Request headers</span></span>

| <span data-ttu-id="673f2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="673f2-118">Name</span></span>          | <span data-ttu-id="673f2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="673f2-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="673f2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="673f2-120">Authorization</span></span> | <span data-ttu-id="673f2-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="673f2-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="673f2-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="673f2-122">Request body</span></span>

<span data-ttu-id="673f2-123">В тексте запроса добавьте представление объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="673f2-123">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="673f2-124">В следующей таблице приведены свойства, необходимые при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="673f2-124">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="673f2-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="673f2-125">Parameter</span></span> | <span data-ttu-id="673f2-126">Тип</span><span class="sxs-lookup"><span data-stu-id="673f2-126">Type</span></span> | <span data-ttu-id="673f2-127">Описание</span><span class="sxs-lookup"><span data-stu-id="673f2-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="673f2-128">displayName</span><span class="sxs-lookup"><span data-stu-id="673f2-128">displayName</span></span> |<span data-ttu-id="673f2-129">string</span><span class="sxs-lookup"><span data-stu-id="673f2-129">string</span></span> |<span data-ttu-id="673f2-130">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="673f2-130">The display name for the role definition.</span></span>|
|<span data-ttu-id="673f2-131">isEnabled</span><span class="sxs-lookup"><span data-stu-id="673f2-131">isEnabled</span></span> |<span data-ttu-id="673f2-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="673f2-132">Boolean</span></span> |<span data-ttu-id="673f2-133">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="673f2-133">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="673f2-134">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="673f2-134">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="673f2-135">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="673f2-135">rolePermissions</span></span> |<span data-ttu-id="673f2-136">Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="673f2-136">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="673f2-137">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="673f2-137">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="673f2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="673f2-138">Response</span></span>

<span data-ttu-id="673f2-139">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="673f2-139">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="673f2-140">Пример</span><span class="sxs-lookup"><span data-stu-id="673f2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="673f2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="673f2-141">Request</span></span>

<span data-ttu-id="673f2-142">Ниже приведен пример создания настраиваемой роли.</span><span class="sxs-lookup"><span data-stu-id="673f2-142">The following is an example of creating a custom role.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="673f2-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="673f2-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="673f2-144">C#</span><span class="sxs-lookup"><span data-stu-id="673f2-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="673f2-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="673f2-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="673f2-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="673f2-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="673f2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="673f2-147">Response</span></span>

<span data-ttu-id="673f2-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="673f2-148">The following is an example of the response.</span></span>

> <span data-ttu-id="673f2-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="673f2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "description": "Update basic properties of application registrations",
    "displayName": "Application Registration Support Administrator",
    "isBuiltIn": false,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "c2cb59a3-2d01-4176-a458-95b0e674966f",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/standard/read",
                "microsoft.directory/applications/basic/update"
            ],
            "condition": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
