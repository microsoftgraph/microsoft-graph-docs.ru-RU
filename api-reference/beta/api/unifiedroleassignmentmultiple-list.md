---
title: Перечисление объектов unifiedRoleAssignmentMultiple
description: Извлечение свойств и связей объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 062cd1d5c39c64eab9018289127eb5c6e691bd44
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2021
ms.locfileid: "52710496"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="6ba41-103">Перечисление объектов unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="6ba41-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="6ba41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ba41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ba41-105">Получите список [объекта unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="6ba41-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="6ba41-106">Используйте это, чтобы получить список назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="6ba41-106">Use this to get a list of role assignments in Microsoft Intune.</span></span> <span data-ttu-id="6ba41-107">Для других Microsoft 365 приложений (например, Azure AD) используйте [унифицированную системуRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6ba41-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ba41-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ba41-108">Permissions</span></span>

<span data-ttu-id="6ba41-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ba41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ba41-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ba41-111">Permission type</span></span> | <span data-ttu-id="6ba41-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ba41-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="6ba41-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ba41-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6ba41-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ba41-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="6ba41-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ba41-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ba41-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ba41-116">Not supported.</span></span> |
| <span data-ttu-id="6ba41-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ba41-117">Application</span></span> | <span data-ttu-id="6ba41-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ba41-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ba41-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ba41-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ba41-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ba41-120">Optional query parameters</span></span>
<span data-ttu-id="6ba41-121">Вы можете фильтровать свойства `roleDefinitionId` или `principalId` свойства.</span><span class="sxs-lookup"><span data-stu-id="6ba41-121">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="6ba41-122">Свойство `roleDefinitionId` может быть как ИД объекта роли, так и объектом шаблона ролей.</span><span class="sxs-lookup"><span data-stu-id="6ba41-122">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="6ba41-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6ba41-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ba41-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ba41-124">Request headers</span></span>

| <span data-ttu-id="6ba41-125">Имя</span><span class="sxs-lookup"><span data-stu-id="6ba41-125">Name</span></span> | <span data-ttu-id="6ba41-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6ba41-126">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="6ba41-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ba41-127">Authorization</span></span> | <span data-ttu-id="6ba41-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ba41-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ba41-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ba41-130">Request body</span></span>

<span data-ttu-id="6ba41-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ba41-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ba41-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ba41-132">Response</span></span>

<span data-ttu-id="6ba41-133">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6ba41-133">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ba41-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6ba41-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ba41-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ba41-135">Request</span></span>

<span data-ttu-id="6ba41-136">Ниже приводится пример запроса:</span><span class="sxs-lookup"><span data-stu-id="6ba41-136">The following is an example of the request:</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="6ba41-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ba41-137">Response</span></span>

<span data-ttu-id="6ba41-138">Ниже приводится пример ответа:</span><span class="sxs-lookup"><span data-stu-id="6ba41-138">The following is an example of the response:</span></span>
> <span data-ttu-id="6ba41-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ba41-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "value": [ 
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
            "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
       },
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "2BNpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SWRD-2",
            "roleDefinitionId": "9e47fc6f-2d7a-464c-944e-d3dd0de522e4",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "53a6c08d-0227-41bd-8bc6-2728df6be749", "a4991fe1-6d7c-427c-969b-bda6df78c458"],
            "appScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0"]
       }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignmentsMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


