---
title: Создание Унифиедроледефинитион
description: Создание нового объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38105a80378ad38fc931abb2e0a94eac0d8a517d
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160249"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="3fa5d-103">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="3fa5d-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="3fa5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fa5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fa5d-105">Создание нового объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="3fa5d-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fa5d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa5d-106">Permissions</span></span>

<span data-ttu-id="3fa5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fa5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3fa5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fa5d-109">Permission type</span></span>                        | <span data-ttu-id="3fa5d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fa5d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3fa5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fa5d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3fa5d-112">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="3fa5d-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="3fa5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fa5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fa5d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-114">Not supported.</span></span> |
| <span data-ttu-id="3fa5d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fa5d-115">Application</span></span>                            | <span data-ttu-id="3fa5d-116">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="3fa5d-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fa5d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fa5d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3fa5d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fa5d-118">Request headers</span></span>

| <span data-ttu-id="3fa5d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3fa5d-119">Name</span></span>          | <span data-ttu-id="3fa5d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3fa5d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3fa5d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fa5d-121">Authorization</span></span> | <span data-ttu-id="3fa5d-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3fa5d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fa5d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3fa5d-123">Request body</span></span>

<span data-ttu-id="3fa5d-124">В тексте запроса добавьте представление объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-124">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="3fa5d-125">В следующей таблице приведены свойства, необходимые при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-125">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="3fa5d-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="3fa5d-126">Parameter</span></span> | <span data-ttu-id="3fa5d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3fa5d-127">Type</span></span> | <span data-ttu-id="3fa5d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3fa5d-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fa5d-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3fa5d-129">displayName</span></span> |<span data-ttu-id="3fa5d-130">string</span><span class="sxs-lookup"><span data-stu-id="3fa5d-130">string</span></span> |<span data-ttu-id="3fa5d-131">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-131">The display name for the role definition.</span></span>|
|<span data-ttu-id="3fa5d-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3fa5d-132">isEnabled</span></span> |<span data-ttu-id="3fa5d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fa5d-133">Boolean</span></span> |<span data-ttu-id="3fa5d-134">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-134">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="3fa5d-135">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-135">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="3fa5d-136">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3fa5d-136">rolePermissions</span></span> |<span data-ttu-id="3fa5d-137">Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3fa5d-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="3fa5d-138">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-138">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="3fa5d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa5d-139">Response</span></span>

<span data-ttu-id="3fa5d-140">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-140">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fa5d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="3fa5d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fa5d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fa5d-142">Request</span></span>

<span data-ttu-id="3fa5d-143">Ниже приведен пример создания настраиваемой роли.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-143">The following is an example of creating a custom role.</span></span>

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

### <a name="response"></a><span data-ttu-id="3fa5d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fa5d-144">Response</span></span>

<span data-ttu-id="3fa5d-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-145">The following is an example of the response.</span></span>
> <span data-ttu-id="3fa5d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fa5d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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