---
title: Создание Унифиедроледефинитион
description: Создание нового объекта Унифиедроледефинитион.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f222f00c6327416cbae95c3f87aab848d8bfda5b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050390"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="f8275-103">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="f8275-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="f8275-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8275-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8275-105">Создание нового объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="f8275-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8275-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8275-106">Permissions</span></span>

<span data-ttu-id="f8275-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8275-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8275-109">Permission type</span></span>                        | <span data-ttu-id="f8275-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8275-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f8275-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8275-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8275-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f8275-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="f8275-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8275-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8275-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8275-114">Not supported.</span></span> |
| <span data-ttu-id="f8275-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8275-115">Application</span></span>                            | <span data-ttu-id="f8275-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="f8275-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8275-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8275-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="f8275-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8275-118">Request headers</span></span>

| <span data-ttu-id="f8275-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f8275-119">Name</span></span>          | <span data-ttu-id="f8275-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f8275-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f8275-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8275-121">Authorization</span></span> | <span data-ttu-id="f8275-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f8275-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8275-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f8275-123">Request body</span></span>

<span data-ttu-id="f8275-124">В тексте запроса добавьте представление объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8275-124">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="f8275-125">В следующей таблице приведены свойства, необходимые при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="f8275-125">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="f8275-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="f8275-126">Parameter</span></span> | <span data-ttu-id="f8275-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f8275-127">Type</span></span> | <span data-ttu-id="f8275-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f8275-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8275-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f8275-129">displayName</span></span> |<span data-ttu-id="f8275-130">string</span><span class="sxs-lookup"><span data-stu-id="f8275-130">string</span></span> |<span data-ttu-id="f8275-131">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="f8275-131">The display name for the role definition.</span></span>|
|<span data-ttu-id="f8275-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f8275-132">isEnabled</span></span> |<span data-ttu-id="f8275-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8275-133">Boolean</span></span> |<span data-ttu-id="f8275-134">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="f8275-134">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="f8275-135">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="f8275-135">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="f8275-136">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f8275-136">rolePermissions</span></span> |<span data-ttu-id="f8275-137">Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f8275-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="f8275-138">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="f8275-138">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="f8275-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8275-139">Response</span></span>

<span data-ttu-id="f8275-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8275-140">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8275-141">Пример</span><span class="sxs-lookup"><span data-stu-id="f8275-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8275-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8275-142">Request</span></span>

<span data-ttu-id="f8275-143">Ниже приведен пример создания настраиваемой роли.</span><span class="sxs-lookup"><span data-stu-id="f8275-143">The following is an example of creating a custom role.</span></span>


# <a name="http"></a>[<span data-ttu-id="f8275-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8275-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f8275-145">C#</span><span class="sxs-lookup"><span data-stu-id="f8275-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8275-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8275-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8275-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8275-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8275-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8275-148">Response</span></span>

<span data-ttu-id="f8275-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f8275-149">The following is an example of the response.</span></span>
> <span data-ttu-id="f8275-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8275-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('c2cb59a3-2d01-4176-a458-95b0e674966f')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
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


