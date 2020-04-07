---
title: Получение Унифиедроледефинитион
description: Получение свойств и связей объекта Унифиедроледефинитион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 28b402aea4ea857912f150ada2665e9094b4bc00
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160319"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="60c87-103">Получение Унифиедроледефинитион</span><span class="sxs-lookup"><span data-stu-id="60c87-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="60c87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60c87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60c87-105">Получение свойств и связей объекта [унифиедроледефинитион](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="60c87-105">Retrieve the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span> <span data-ttu-id="60c87-106">В настоящее время "каталог" является единственным поддерживаемым приложением RBAC.</span><span class="sxs-lookup"><span data-stu-id="60c87-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="60c87-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60c87-107">Permissions</span></span>

<span data-ttu-id="60c87-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60c87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60c87-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60c87-110">Permission type</span></span>      | <span data-ttu-id="60c87-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60c87-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60c87-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60c87-112">Delegated (work or school account)</span></span> | <span data-ttu-id="60c87-113">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="60c87-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="60c87-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60c87-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60c87-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60c87-115">Not supported.</span></span>    |
|<span data-ttu-id="60c87-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60c87-116">Application</span></span> | <span data-ttu-id="60c87-117">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="60c87-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60c87-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60c87-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/{rbacApplication}/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60c87-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60c87-119">Optional query parameters</span></span>

<span data-ttu-id="60c87-120">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="60c87-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="60c87-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="60c87-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="60c87-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60c87-122">Request headers</span></span>

| <span data-ttu-id="60c87-123">Имя</span><span class="sxs-lookup"><span data-stu-id="60c87-123">Name</span></span>      |<span data-ttu-id="60c87-124">Описание</span><span class="sxs-lookup"><span data-stu-id="60c87-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="60c87-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="60c87-125">Authorization</span></span> | <span data-ttu-id="60c87-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="60c87-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="60c87-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60c87-127">Request body</span></span>

<span data-ttu-id="60c87-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60c87-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60c87-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="60c87-129">Response</span></span>

<span data-ttu-id="60c87-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60c87-130">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60c87-131">Пример</span><span class="sxs-lookup"><span data-stu-id="60c87-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="60c87-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="60c87-132">Request</span></span>

<span data-ttu-id="60c87-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60c87-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```

### <a name="response"></a><span data-ttu-id="60c87-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="60c87-134">Response</span></span>

<span data-ttu-id="60c87-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60c87-135">The following is an example of the response.</span></span>

> <span data-ttu-id="60c87-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60c87-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "f189965f-f560-4c59-9101-933d4c87a91a",
    "description": "Allows reading Application Registrations",
    "displayName": "Application Registration Reader",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "429c3819-053d-4250-9926-4c7dcb18ae17",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/allProperties/read"
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
  "description": "Get unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->