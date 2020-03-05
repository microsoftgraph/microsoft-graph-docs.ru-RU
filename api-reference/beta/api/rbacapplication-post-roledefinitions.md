---
title: Создание Унифиедроледефинитион
description: Создание нового объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ed5059aaab1e89ddc1ce89a78c21efaaa9a34ad6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454497"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="6d009-103">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="6d009-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="6d009-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6d009-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d009-105">Создание нового объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="6d009-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d009-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d009-106">Permissions</span></span>

<span data-ttu-id="6d009-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d009-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d009-109">Permission type</span></span>                        | <span data-ttu-id="6d009-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d009-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6d009-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d009-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d009-112">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="6d009-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="6d009-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d009-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d009-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d009-114">Not supported.</span></span> |
| <span data-ttu-id="6d009-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d009-115">Application</span></span>                            | <span data-ttu-id="6d009-116">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="6d009-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d009-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d009-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="6d009-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d009-118">Request headers</span></span>

| <span data-ttu-id="6d009-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6d009-119">Name</span></span>          | <span data-ttu-id="6d009-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6d009-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6d009-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d009-121">Authorization</span></span> | <span data-ttu-id="6d009-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6d009-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d009-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d009-123">Request body</span></span>

<span data-ttu-id="6d009-124">В тексте запроса добавьте представление объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d009-124">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="6d009-125">В следующей таблице приведены свойства, необходимые при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="6d009-125">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="6d009-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="6d009-126">Parameter</span></span> | <span data-ttu-id="6d009-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6d009-127">Type</span></span> | <span data-ttu-id="6d009-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6d009-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d009-129">displayName</span><span class="sxs-lookup"><span data-stu-id="6d009-129">displayName</span></span> |<span data-ttu-id="6d009-130">string</span><span class="sxs-lookup"><span data-stu-id="6d009-130">string</span></span> |<span data-ttu-id="6d009-131">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="6d009-131">The display name for the role definition.</span></span>|
|<span data-ttu-id="6d009-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6d009-132">isEnabled</span></span> |<span data-ttu-id="6d009-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d009-133">Boolean</span></span> |<span data-ttu-id="6d009-134">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="6d009-134">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="6d009-135">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="6d009-135">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="6d009-136">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="6d009-136">rolePermissions</span></span> |<span data-ttu-id="6d009-137">Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="6d009-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="6d009-138">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="6d009-138">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="6d009-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d009-139">Response</span></span>

<span data-ttu-id="6d009-140">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d009-140">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d009-141">Пример</span><span class="sxs-lookup"><span data-stu-id="6d009-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d009-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d009-142">Request</span></span>

<span data-ttu-id="6d009-143">Ниже приведен пример создания настраиваемой роли.</span><span class="sxs-lookup"><span data-stu-id="6d009-143">The following is an example of creating a custom role.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d009-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d009-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6d009-145">C#</span><span class="sxs-lookup"><span data-stu-id="6d009-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d009-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d009-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d009-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d009-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d009-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d009-148">Response</span></span>

<span data-ttu-id="6d009-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6d009-149">The following is an example of the response.</span></span>

> <span data-ttu-id="6d009-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d009-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
