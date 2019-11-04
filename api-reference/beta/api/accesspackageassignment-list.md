---
title: Список Акцесспаккажеассигнментс
description: Получение списка объектов акцесспаккажеассигнмент.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ed838b01364e5616db6ed8b2236dc0b5593d9ff
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936064"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="6531e-103">Список Акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="6531e-103">List accessPackageAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6531e-104">Получение списка объектов [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) в [службе управления обслуживанием Azure AD](../resources/entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="6531e-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span>  <span data-ttu-id="6531e-105">В полученном списке содержатся все назначения, текущие и просроченные, которые вызывающий абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="6531e-105">The resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="6531e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6531e-106">Permissions</span></span>

<span data-ttu-id="6531e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6531e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6531e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6531e-109">Permission type</span></span>                        | <span data-ttu-id="6531e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6531e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6531e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6531e-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="6531e-112">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6531e-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6531e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6531e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6531e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6531e-114">Not supported.</span></span> |
| <span data-ttu-id="6531e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6531e-115">Application</span></span>                            | <span data-ttu-id="6531e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6531e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6531e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6531e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6531e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6531e-118">Optional query parameters</span></span>

<span data-ttu-id="6531e-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6531e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6531e-120">Например, чтобы получить только доставленные назначения, можно включить запрос `$filter=assignmentState eq 'Delivered'`.</span><span class="sxs-lookup"><span data-stu-id="6531e-120">For example, to retrieve only Delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span>
<span data-ttu-id="6531e-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6531e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6531e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6531e-122">Request headers</span></span>

| <span data-ttu-id="6531e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6531e-123">Name</span></span>      |<span data-ttu-id="6531e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6531e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6531e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6531e-125">Authorization</span></span> | <span data-ttu-id="6531e-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="6531e-126">Bearer \{token\}.</span></span> <span data-ttu-id="6531e-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="6531e-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6531e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6531e-128">Request body</span></span>

<span data-ttu-id="6531e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6531e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6531e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6531e-130">Response</span></span>

<span data-ttu-id="6531e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6531e-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6531e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="6531e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6531e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6531e-133">Request</span></span>

<span data-ttu-id="6531e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6531e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```

### <a name="response"></a><span data-ttu-id="6531e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6531e-135">Response</span></span>

<span data-ttu-id="6531e-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6531e-136">The following is an example of the response.</span></span>

> <span data-ttu-id="6531e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6531e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
      "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
      "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
      "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
      "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
      "assignmentStatus": "ExpiredNotificationTriggered",
      "assignmentState": "Expired",
      "isExtended": false,
      "expiredDateTime": "2019-04-25T23:45:40.42Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
