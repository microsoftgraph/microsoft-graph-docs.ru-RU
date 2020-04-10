---
title: Перечисление объектов unifiedRoleAssignmentMultiple
description: Получение свойств и связей объекта Унифиедролеассигнментмултипле.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 174c848da527fb0f32bd3102e01dfcff5baffa40
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218978"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="0f87e-103">Перечисление объектов unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0f87e-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="0f87e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f87e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f87e-105">Получение списка объектов [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="0f87e-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="0f87e-106">Используйте эту возможность для получения списка назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="0f87e-106">Use this to get a list of role assignments in Microsoft Intune.</span></span> <span data-ttu-id="0f87e-107">Для других приложений Микрсофт 365 (например, Azure AD) используйте [унифиедролеассигнмент](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0f87e-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f87e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f87e-108">Permissions</span></span>

<span data-ttu-id="0f87e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f87e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f87e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f87e-111">Permission type</span></span> | <span data-ttu-id="0f87e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f87e-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="0f87e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f87e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0f87e-114">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="0f87e-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="0f87e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f87e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f87e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f87e-116">Not supported.</span></span> |
| <span data-ttu-id="0f87e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f87e-117">Application</span></span> | <span data-ttu-id="0f87e-118">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0f87e-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f87e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f87e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f87e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0f87e-120">Optional query parameters</span></span>

<span data-ttu-id="0f87e-121">Для `$filter` выполнения этой операции требуется параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="0f87e-121">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="0f87e-122">Вы можете отфильтровать `roleDefinitionId` по `principalId` свойствам или.</span><span class="sxs-lookup"><span data-stu-id="0f87e-122">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="0f87e-123">`roleDefinitionId` Свойство может быть идентификатором объекта Role или шаблоном роли.</span><span class="sxs-lookup"><span data-stu-id="0f87e-123">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="0f87e-124">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0f87e-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f87e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f87e-125">Request headers</span></span>

| <span data-ttu-id="0f87e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="0f87e-126">Name</span></span> | <span data-ttu-id="0f87e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="0f87e-127">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0f87e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f87e-128">Authorization</span></span> | <span data-ttu-id="0f87e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f87e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f87e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f87e-131">Request body</span></span>

<span data-ttu-id="0f87e-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f87e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f87e-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f87e-133">Response</span></span>

<span data-ttu-id="0f87e-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f87e-134">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f87e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0f87e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f87e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f87e-136">Request</span></span>

<span data-ttu-id="0f87e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f87e-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="0f87e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f87e-138">Response</span></span>

<span data-ttu-id="0f87e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0f87e-139">The following is an example of the response.</span></span>
> <span data-ttu-id="0f87e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f87e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
