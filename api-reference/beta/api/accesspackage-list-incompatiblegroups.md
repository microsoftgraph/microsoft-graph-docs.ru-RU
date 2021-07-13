---
title: Несовместимые группы списка
description: Извлечение списка групп, права доступа которых несовместимы с определенным пакетом доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1c41cafb01ba86975c2dcbde12272951123d1eea
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401163"
---
# <a name="list-incompatiblegroups"></a><span data-ttu-id="ae25c-103">Несовместимые группы списка</span><span class="sxs-lookup"><span data-stu-id="ae25c-103">List incompatibleGroups</span></span>

<span data-ttu-id="ae25c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae25c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae25c-105">Извлечение списка [объектов группы,](../resources/group.md) которые были отмечены как несовместимые в [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="ae25c-105">Retrieve a list of the [group](../resources/group.md) objects that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="ae25c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae25c-106">Permissions</span></span>

<span data-ttu-id="ae25c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae25c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae25c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae25c-109">Permission type</span></span>                        | <span data-ttu-id="ae25c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae25c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ae25c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae25c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae25c-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae25c-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ae25c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae25c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae25c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae25c-114">Not supported.</span></span> |
| <span data-ttu-id="ae25c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ae25c-115">Application</span></span>                            | <span data-ttu-id="ae25c-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae25c-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae25c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae25c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/incompatibleGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae25c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae25c-118">Optional query parameters</span></span>

<span data-ttu-id="ae25c-119">Этот метод поддерживает параметры запроса OData для прогона на стороне сервера с помощью большого отклика.</span><span class="sxs-lookup"><span data-stu-id="ae25c-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="ae25c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ae25c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae25c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae25c-121">Request headers</span></span>

| <span data-ttu-id="ae25c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ae25c-122">Name</span></span>      |<span data-ttu-id="ae25c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ae25c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae25c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae25c-124">Authorization</span></span> | <span data-ttu-id="ae25c-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae25c-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae25c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae25c-127">Request body</span></span>

<span data-ttu-id="ae25c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae25c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae25c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae25c-129">Response</span></span>

<span data-ttu-id="ae25c-130">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="ae25c-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae25c-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae25c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae25c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae25c-132">Request</span></span>

<span data-ttu-id="ae25c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae25c-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_incompatiblegroups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups
```

### <a name="response"></a><span data-ttu-id="ae25c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae25c-134">Response</span></span>

<span data-ttu-id="ae25c-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ae25c-135">The following is an example of the response.</span></span>

> <span data-ttu-id="ae25c-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ae25c-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "a743348f-5667-41a4-89a3-5ad8a94da5d2",
      "displayName": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List incompatibleGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

