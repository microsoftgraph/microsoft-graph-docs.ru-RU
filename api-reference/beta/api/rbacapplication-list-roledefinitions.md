---
title: Список Унифиедроледефинитионс
description: Получение списка объектов Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 642b5582d49930e340d8d879c9b65f7ff4b05e2a
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437701"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="9700a-103">Список Унифиедроледефинитионс</span><span class="sxs-lookup"><span data-stu-id="9700a-103">List unifiedRoleDefinitions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9700a-104">Получение списка объектов [унифиедроледефинитион](../resources/unifiedroledefinition.md) для поставщика.</span><span class="sxs-lookup"><span data-stu-id="9700a-104">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="9700a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9700a-105">Permissions</span></span>

<span data-ttu-id="9700a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9700a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9700a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9700a-108">Permission type</span></span>      | <span data-ttu-id="9700a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9700a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9700a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9700a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9700a-111">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="9700a-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9700a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9700a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9700a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9700a-113">Not supported.</span></span>    |
|<span data-ttu-id="9700a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9700a-114">Application</span></span> | <span data-ttu-id="9700a-115">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9700a-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9700a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9700a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9700a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9700a-117">Optional query parameters</span></span>
<span data-ttu-id="9700a-118">Этот метод поддерживает `$filter` `id`, `displayName`и `isBuiltIn`.</span><span class="sxs-lookup"><span data-stu-id="9700a-118">This method supports `$filter` on `id`, `displayName`, and `isBuiltIn`.</span></span> <span data-ttu-id="9700a-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9700a-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9700a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9700a-120">Request headers</span></span>

| <span data-ttu-id="9700a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9700a-121">Name</span></span>      |<span data-ttu-id="9700a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9700a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9700a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9700a-123">Authorization</span></span> | <span data-ttu-id="9700a-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9700a-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9700a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9700a-125">Request body</span></span>

<span data-ttu-id="9700a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9700a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9700a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9700a-127">Response</span></span>

<span data-ttu-id="9700a-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9700a-128">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9700a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9700a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9700a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9700a-130">Request</span></span>

<span data-ttu-id="9700a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9700a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="9700a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9700a-132">Response</span></span>

<span data-ttu-id="9700a-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9700a-133">The following is an example of the response.</span></span>

> <span data-ttu-id="9700a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9700a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
