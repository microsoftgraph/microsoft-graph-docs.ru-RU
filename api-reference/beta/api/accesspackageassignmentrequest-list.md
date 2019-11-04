---
title: Список Акцесспаккажеассигнментрекуестс
description: Получение списка объектов Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d97b0f7c3f06652a7d22d0b803d471b95a233e62
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936055"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="48bd8-103">Список Акцесспаккажеассигнментрекуестс</span><span class="sxs-lookup"><span data-stu-id="48bd8-103">List accessPackageAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48bd8-104">Получение списка объектов [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в [службе управления обслуживанием Azure AD](../resources/entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="48bd8-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="48bd8-105">Полученный список включает все запросы на начисление, текущие и срок действия которых просрочены, которые вызывающий абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="48bd8-105">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="48bd8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48bd8-106">Permissions</span></span>

<span data-ttu-id="48bd8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48bd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48bd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48bd8-109">Permission type</span></span>                        | <span data-ttu-id="48bd8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48bd8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48bd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48bd8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48bd8-112">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="48bd8-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="48bd8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48bd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48bd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48bd8-114">Not supported.</span></span> |
| <span data-ttu-id="48bd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48bd8-115">Application</span></span>                            | <span data-ttu-id="48bd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48bd8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48bd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48bd8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="48bd8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48bd8-118">Optional query parameters</span></span>

<span data-ttu-id="48bd8-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48bd8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="48bd8-120">Например, чтобы получить пакет доступа для каждого запроса, включите `$expand=accessPackage` в запрос.</span><span class="sxs-lookup"><span data-stu-id="48bd8-120">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="48bd8-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="48bd8-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="48bd8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48bd8-122">Request headers</span></span>

| <span data-ttu-id="48bd8-123">Имя</span><span class="sxs-lookup"><span data-stu-id="48bd8-123">Name</span></span>      |<span data-ttu-id="48bd8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="48bd8-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48bd8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="48bd8-125">Authorization</span></span> | <span data-ttu-id="48bd8-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="48bd8-126">Bearer \{token\}.</span></span> <span data-ttu-id="48bd8-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="48bd8-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48bd8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48bd8-128">Request body</span></span>

<span data-ttu-id="48bd8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48bd8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48bd8-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="48bd8-130">Response</span></span>

<span data-ttu-id="48bd8-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48bd8-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48bd8-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="48bd8-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48bd8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="48bd8-133">Request</span></span>

<span data-ttu-id="48bd8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48bd8-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

### <a name="response"></a><span data-ttu-id="48bd8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="48bd8-135">Response</span></span>

<span data-ttu-id="48bd8-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48bd8-136">The following is an example of the response.</span></span>

> <span data-ttu-id="48bd8-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48bd8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "433dafca-5047-4614-95f7-a03510b1ded3",
      "requestType": "AdminAdd",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "isValidationOnly": false,
      "createdDateTime": "2019-10-25T22:55:11.623Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
