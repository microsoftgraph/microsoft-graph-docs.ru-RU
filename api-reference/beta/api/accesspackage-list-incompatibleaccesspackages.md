---
title: Список несовместимыхAccessPackages
description: Извлечение списка accesspackages, права доступа которых несовместимы с определенным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fc30ee9ae6a80b04820b363dea87f376e5db638b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401166"
---
# <a name="list-incompatibleaccesspackages"></a><span data-ttu-id="46545-103">Список несовместимыхAccessPackages</span><span class="sxs-lookup"><span data-stu-id="46545-103">List incompatibleAccessPackages</span></span>

<span data-ttu-id="46545-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46545-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46545-105">Извлечение списка объектов [accessPackage,](../resources/accesspackage.md) которые были отмечены как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="46545-105">Retrieve a list of the [accessPackage](../resources/accesspackage.md) objects that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="46545-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46545-106">Permissions</span></span>

<span data-ttu-id="46545-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46545-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46545-109">Permission type</span></span>                        | <span data-ttu-id="46545-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46545-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46545-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46545-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="46545-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46545-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="46545-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46545-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46545-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46545-114">Not supported.</span></span> |
| <span data-ttu-id="46545-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="46545-115">Application</span></span>                            | <span data-ttu-id="46545-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46545-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46545-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46545-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/incompatibleAccessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46545-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="46545-118">Optional query parameters</span></span>

<span data-ttu-id="46545-119">Этот метод поддерживает параметры запроса OData для прогона на стороне сервера с помощью большого отклика.</span><span class="sxs-lookup"><span data-stu-id="46545-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="46545-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="46545-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="46545-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46545-121">Request headers</span></span>

| <span data-ttu-id="46545-122">Имя</span><span class="sxs-lookup"><span data-stu-id="46545-122">Name</span></span>      |<span data-ttu-id="46545-123">Описание</span><span class="sxs-lookup"><span data-stu-id="46545-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46545-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46545-124">Authorization</span></span> | <span data-ttu-id="46545-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46545-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46545-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46545-127">Request body</span></span>

<span data-ttu-id="46545-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46545-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46545-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="46545-129">Response</span></span>

<span data-ttu-id="46545-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessPackage](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46545-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46545-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="46545-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46545-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="46545-132">Request</span></span>

<span data-ttu-id="46545-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46545-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_incompatibleaccesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages
### Response

The following is an example of the response.

> **Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
      "catalogId": "c955f54f-e248-4155-b314-0bdd63f5aae9",
      "displayName": "accesspackage"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List incompatibleAccessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

