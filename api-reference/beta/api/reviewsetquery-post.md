---
title: Создание Ревиевсеткуери
description: Используйте этот API для создания нового Ревиевсеткуери.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: e318c99408fdd0cb5e884a869cbbc2de8ce53c1b
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510273"
---
# <a name="create-reviewsetquery"></a><span data-ttu-id="f1121-103">Создание Ревиевсеткуери</span><span class="sxs-lookup"><span data-stu-id="f1121-103">Create reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1121-104">Создание нового объекта [ревиевсеткуери](../resources/reviewsetquery.md) .</span><span class="sxs-lookup"><span data-stu-id="f1121-104">Create a new [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1121-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1121-105">Permissions</span></span>

<span data-ttu-id="f1121-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1121-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f1121-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1121-108">Permission type</span></span>                        | <span data-ttu-id="f1121-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1121-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f1121-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1121-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1121-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="f1121-111">User.Read</span></span> |
| <span data-ttu-id="f1121-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1121-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1121-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1121-113">Not supported.</span></span> |
| <span data-ttu-id="f1121-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1121-114">Application</span></span>                            | <span data-ttu-id="f1121-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1121-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1121-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1121-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="request-headers"></a><span data-ttu-id="f1121-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1121-117">Request headers</span></span>

| <span data-ttu-id="f1121-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f1121-118">Name</span></span>          | <span data-ttu-id="f1121-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f1121-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f1121-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1121-120">Authorization</span></span> | <span data-ttu-id="f1121-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1121-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1121-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1121-123">Request body</span></span>

<span data-ttu-id="f1121-124">В тексте запроса добавьте представление объекта [ревиевсеткуери](../resources/reviewsetquery.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1121-124">In the request body, supply a JSON representation of [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span> <span data-ttu-id="f1121-125">В следующей таблице перечислены обязательные свойства.</span><span class="sxs-lookup"><span data-stu-id="f1121-125">The following table lists the required properties.</span></span>

| <span data-ttu-id="f1121-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1121-126">Property</span></span>     | <span data-ttu-id="f1121-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f1121-127">Type</span></span>        | <span data-ttu-id="f1121-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f1121-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f1121-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f1121-129">displayName</span></span>  | <span data-ttu-id="f1121-130">string</span><span class="sxs-lookup"><span data-stu-id="f1121-130">string</span></span>      | <span data-ttu-id="f1121-131">Имя запроса на проверку набора</span><span class="sxs-lookup"><span data-stu-id="f1121-131">The name of the review set query</span></span> |

## <a name="response"></a><span data-ttu-id="f1121-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1121-132">Response</span></span>

<span data-ttu-id="f1121-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [ревиевсеткуери](../resources/reviewsetquery.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1121-133">If successful, this method returns a `201 Created` response code and a new [reviewSetQuery](../resources/reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1121-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="f1121-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1121-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1121-135">Request</span></span>

<span data-ttu-id="f1121-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1121-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reviewsetquery"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
Content-type: application/json

{
     "displayName" : "My Query 1",
     "query": "(subject:\"Quarterly Financials\")"
}
```

### <a name="response"></a><span data-ttu-id="f1121-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1121-137">Response</span></span>

<span data-ttu-id="f1121-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f1121-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f1121-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1121-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries/$entity",
    "id": "6b5358b0-2ce2-4369-b9cf-65392fe56807",
    "displayName": "My Query 1",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-09T09:05:12.3756813Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-03-09T09:05:12.3756813Z",
    "query": "(subject:\"Quarterly Financials\")"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
