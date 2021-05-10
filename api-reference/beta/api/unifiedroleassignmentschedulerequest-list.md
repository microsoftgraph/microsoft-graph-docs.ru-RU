---
title: Список unifiedRoleAssignmentScheduleRequests
description: Получите список объектов unifiedRoleAssignmentScheduleRequest и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29e3c448dc96cfc1dfacad1a3eece2dbe5220688
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299772"
---
# <a name="list-unifiedroleassignmentschedulerequests"></a><span data-ttu-id="12252-103">Список unifiedRoleAssignmentScheduleRequests</span><span class="sxs-lookup"><span data-stu-id="12252-103">List unifiedRoleAssignmentScheduleRequests</span></span>

<span data-ttu-id="12252-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12252-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12252-105">Получите список объектов [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="12252-105">Get a list of the [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="12252-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12252-106">Permissions</span></span>

<span data-ttu-id="12252-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12252-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12252-109">Permission type</span></span>                        | <span data-ttu-id="12252-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12252-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="12252-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12252-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="12252-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="12252-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>          |
| <span data-ttu-id="12252-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12252-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12252-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="12252-114">Not supported</span></span>                               |
| <span data-ttu-id="12252-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12252-115">Application</span></span>                            | <span data-ttu-id="12252-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="12252-116">PrivilegedAccess.Read.AzureAD</span></span>               |

## <a name="http-request"></a><span data-ttu-id="12252-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12252-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /roleManagement/directory/roleAssignmentScheduleRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12252-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12252-118">Optional query parameters</span></span>

<span data-ttu-id="12252-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="12252-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="12252-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="12252-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="12252-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12252-121">Request headers</span></span>

| <span data-ttu-id="12252-122">Имя</span><span class="sxs-lookup"><span data-stu-id="12252-122">Name</span></span>          | <span data-ttu-id="12252-123">Описание</span><span class="sxs-lookup"><span data-stu-id="12252-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="12252-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12252-124">Authorization</span></span> | <span data-ttu-id="12252-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12252-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12252-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12252-127">Request body</span></span>

<span data-ttu-id="12252-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12252-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12252-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="12252-129">Response</span></span>

<span data-ttu-id="12252-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="12252-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12252-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="12252-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12252-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="12252-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentschedulerequest"
}
-->

```http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests
```

### <a name="response"></a><span data-ttu-id="12252-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="12252-133">Response</span></span>

<span data-ttu-id="12252-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="12252-134">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleAssignmentScheduleRequest)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "c13ee236-e236-c13e-36e2-3ec136e23ec1",
      "action": "String",
      "principalId": "String",
      "roleDefinitionId": "String",
      "directoryScopeId": "String",
      "appScopeId": "String",
      "isValidationOnly": "Boolean",
      "targetScheduleId": "String",
      "justification": "String",
      "scheduleInfo": {
        "@odata.type": "microsoft.graph.requestSchedule"
      },
      "ticketInfo": {
        "@odata.type": "microsoft.graph.ticketInfo"
      }
    }
  ]
}
```
