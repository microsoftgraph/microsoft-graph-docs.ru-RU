---
title: Создание Унифиедроледефинитион
description: Создание нового объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 803f21d56a6d02a64013a711cf5419996eb73de8
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437715"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="3b822-103">Создание Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="3b822-103">Create unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b822-104">Создание нового объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="3b822-104">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b822-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b822-105">Permissions</span></span>

<span data-ttu-id="3b822-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b822-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b822-108">Permission type</span></span>                        | <span data-ttu-id="3b822-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b822-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3b822-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b822-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b822-111">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="3b822-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="3b822-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b822-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b822-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b822-113">Not supported.</span></span> |
| <span data-ttu-id="3b822-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b822-114">Application</span></span>                            | <span data-ttu-id="3b822-115">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="3b822-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b822-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b822-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="3b822-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b822-117">Request headers</span></span>

| <span data-ttu-id="3b822-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3b822-118">Name</span></span>          | <span data-ttu-id="3b822-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3b822-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3b822-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b822-120">Authorization</span></span> | <span data-ttu-id="3b822-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3b822-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b822-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b822-122">Request body</span></span>

<span data-ttu-id="3b822-123">В тексте запроса добавьте представление объекта [унифиедроледефинитион](../resources/unifiedroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b822-123">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="3b822-124">В следующей таблице приведены свойства, необходимые при создании объекта roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="3b822-124">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="3b822-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="3b822-125">Parameter</span></span> | <span data-ttu-id="3b822-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3b822-126">Type</span></span> | <span data-ttu-id="3b822-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3b822-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b822-128">displayName</span><span class="sxs-lookup"><span data-stu-id="3b822-128">displayName</span></span> |<span data-ttu-id="3b822-129">string</span><span class="sxs-lookup"><span data-stu-id="3b822-129">string</span></span> |<span data-ttu-id="3b822-130">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="3b822-130">The display name for the role definition.</span></span>|
|<span data-ttu-id="3b822-131">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3b822-131">isEnabled</span></span> |<span data-ttu-id="3b822-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b822-132">Boolean</span></span> |<span data-ttu-id="3b822-133">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="3b822-133">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="3b822-134">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="3b822-134">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="3b822-135">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="3b822-135">rolePermissions</span></span> |<span data-ttu-id="3b822-136">Коллекция [унифиедролепермиссион](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="3b822-136">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="3b822-137">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="3b822-137">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="3b822-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b822-138">Response</span></span>

<span data-ttu-id="3b822-139">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b822-139">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b822-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3b822-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b822-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b822-141">Request</span></span>

<span data-ttu-id="3b822-142">Ниже приведен пример создания настраиваемой роли.</span><span class="sxs-lookup"><span data-stu-id="3b822-142">The following is an example of creating a custom role.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b822-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b822-143">Response</span></span>

<span data-ttu-id="3b822-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b822-144">The following is an example of the response.</span></span>

> <span data-ttu-id="3b822-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b822-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
