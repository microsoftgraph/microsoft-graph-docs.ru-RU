---
title: Получение Акцесспаккажеассигнментрекуест
description: Получение свойств и связей объекта Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5768664edbdce00b8004ee9031520fdcc9331ef3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936056"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="ef1c9-103">Получение Акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="ef1c9-103">Get accessPackageAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef1c9-104">В разделе [Управление обслуживанием Azure AD](../resources/entitlementmanagement-root.md)извлекаются свойства и связи объекта [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ef1c9-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef1c9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef1c9-105">Permissions</span></span>

<span data-ttu-id="ef1c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef1c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef1c9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef1c9-108">Permission type</span></span>                        | <span data-ttu-id="ef1c9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef1c9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ef1c9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef1c9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef1c9-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef1c9-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="ef1c9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef1c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef1c9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-113">Not supported.</span></span> |
| <span data-ttu-id="ef1c9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef1c9-114">Application</span></span>                            | <span data-ttu-id="ef1c9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef1c9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef1c9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef1c9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef1c9-117">Optional query parameters</span></span>

<span data-ttu-id="ef1c9-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ef1c9-119">Например, чтобы получить запрошенный пакет Access, включите `$expand=accessPackage` его в запрос.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-119">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="ef1c9-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ef1c9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef1c9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef1c9-121">Request headers</span></span>

| <span data-ttu-id="ef1c9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ef1c9-122">Name</span></span>      |<span data-ttu-id="ef1c9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ef1c9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef1c9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef1c9-124">Authorization</span></span> | <span data-ttu-id="ef1c9-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-125">Bearer \{token\}.</span></span> <span data-ttu-id="ef1c9-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef1c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef1c9-127">Request body</span></span>

<span data-ttu-id="ef1c9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef1c9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef1c9-129">Response</span></span>

<span data-ttu-id="ef1c9-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef1c9-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef1c9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef1c9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef1c9-132">Request</span></span>

<span data-ttu-id="ef1c9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

### <a name="response"></a><span data-ttu-id="ef1c9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef1c9-134">Response</span></span>

<span data-ttu-id="ef1c9-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-135">The following is an example of the response.</span></span>

> <span data-ttu-id="ef1c9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef1c9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "433dafca-5047-4614-95f7-a03510b1ded3",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "createdDateTime": "2019-10-25T22:55:11.623Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
