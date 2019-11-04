---
title: Получение Акцесспаккаже
description: Получение свойств и связей объекта Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 85ca036b24b8ff103fab130f8d118cac8cca96da
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936066"
---
# <a name="get-accesspackage"></a><span data-ttu-id="2ccf3-103">Получение Акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="2ccf3-103">Get accessPackage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ccf3-104">Получение свойств и связей объекта [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="2ccf3-104">Retrieve the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ccf3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ccf3-105">Permissions</span></span>

<span data-ttu-id="2ccf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ccf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ccf3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ccf3-108">Permission type</span></span>                        | <span data-ttu-id="2ccf3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ccf3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ccf3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ccf3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ccf3-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2ccf3-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="2ccf3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ccf3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ccf3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-113">Not supported.</span></span> |
| <span data-ttu-id="2ccf3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ccf3-114">Application</span></span>                            | <span data-ttu-id="2ccf3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ccf3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ccf3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ccf3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2ccf3-117">Optional query parameters</span></span>

<span data-ttu-id="2ccf3-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ccf3-119">Например, чтобы получить доступ к политикам пакетов доступа, `$expand=accessPackageAssignmentPolicies`добавьте.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-119">For example, to retrieve the access package policies, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="2ccf3-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2ccf3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ccf3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ccf3-121">Request headers</span></span>

| <span data-ttu-id="2ccf3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2ccf3-122">Name</span></span>      |<span data-ttu-id="2ccf3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2ccf3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ccf3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ccf3-124">Authorization</span></span> | <span data-ttu-id="2ccf3-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-125">Bearer \{token\}.</span></span> <span data-ttu-id="2ccf3-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ccf3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ccf3-127">Request body</span></span>

<span data-ttu-id="2ccf3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ccf3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ccf3-129">Response</span></span>

<span data-ttu-id="2ccf3-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккаже](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-130">If successful, this method returns a `200 OK` response code and the requested [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ccf3-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ccf3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ccf3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ccf3-132">Request</span></span>

<span data-ttu-id="2ccf3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```

### <a name="response"></a><span data-ttu-id="2ccf3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ccf3-134">Response</span></span>

<span data-ttu-id="2ccf3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-135">The following is an example of the response.</span></span>

> <span data-ttu-id="2ccf3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ccf3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
