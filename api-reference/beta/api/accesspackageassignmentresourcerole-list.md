---
title: Список Акцесспаккажеассигнментресаурцеролес
description: Получение списка объектов Акцесспаккажеассигнментресаурцерроле.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 16d2e91b00832b4745682861573985cc5bde27fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936048"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="54fd3-103">Список Акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="54fd3-103">List accessPackageAssignmentResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54fd3-104">Получение списка объектов [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="54fd3-104">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="54fd3-105">Полученный список включает все роли ресурсов для всех назначений, которые абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="54fd3-105">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="54fd3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54fd3-106">Permissions</span></span>

<span data-ttu-id="54fd3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54fd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54fd3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54fd3-109">Permission type</span></span>                        | <span data-ttu-id="54fd3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54fd3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54fd3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54fd3-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="54fd3-112">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="54fd3-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="54fd3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54fd3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54fd3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54fd3-114">Not supported.</span></span> |
| <span data-ttu-id="54fd3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54fd3-115">Application</span></span>                            | <span data-ttu-id="54fd3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54fd3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54fd3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54fd3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54fd3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54fd3-118">Optional query parameters</span></span>

<span data-ttu-id="54fd3-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="54fd3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="54fd3-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="54fd3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="54fd3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54fd3-121">Request headers</span></span>

| <span data-ttu-id="54fd3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="54fd3-122">Name</span></span>      |<span data-ttu-id="54fd3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="54fd3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54fd3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="54fd3-124">Authorization</span></span> | <span data-ttu-id="54fd3-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="54fd3-125">Bearer \{token\}.</span></span> <span data-ttu-id="54fd3-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="54fd3-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54fd3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54fd3-127">Request body</span></span>

<span data-ttu-id="54fd3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54fd3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54fd3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="54fd3-129">Response</span></span>

<span data-ttu-id="54fd3-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54fd3-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54fd3-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="54fd3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54fd3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="54fd3-132">Request</span></span>

<span data-ttu-id="54fd3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54fd3-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

### <a name="response"></a><span data-ttu-id="54fd3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="54fd3-134">Response</span></span>

<span data-ttu-id="54fd3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="54fd3-135">The following is an example of the response.</span></span>

> <span data-ttu-id="54fd3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54fd3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
      "originId": "originId-value",
      "originSystem": "SharePointOnline",
      "status": "Fulfilled"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
