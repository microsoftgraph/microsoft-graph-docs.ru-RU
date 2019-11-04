---
title: Список Акцесспаккажес
description: Получение списка объектов Акцесспаккаже.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 219d5a53c6b20666c4727430ccae6bebee9bb325
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936073"
---
# <a name="list-accesspackages"></a><span data-ttu-id="6265f-103">Список Акцесспаккажес</span><span class="sxs-lookup"><span data-stu-id="6265f-103">List accessPackages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6265f-104">Получение списка объектов [акцесспаккаже](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="6265f-104">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="6265f-105">Полученный список включает все пакеты доступа, которые абонент имеет доступ для чтения, во всех каталогах.</span><span class="sxs-lookup"><span data-stu-id="6265f-105">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="6265f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6265f-106">Permissions</span></span>

<span data-ttu-id="6265f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6265f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6265f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6265f-109">Permission type</span></span>                        | <span data-ttu-id="6265f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6265f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6265f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6265f-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="6265f-112">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6265f-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6265f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6265f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6265f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6265f-114">Not supported.</span></span> |
| <span data-ttu-id="6265f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6265f-115">Application</span></span>                            | <span data-ttu-id="6265f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6265f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6265f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6265f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6265f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6265f-118">Optional query parameters</span></span>

<span data-ttu-id="6265f-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6265f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6265f-120">Например, чтобы получить политики пакетов доступа для каждого пакета Access, добавьте `$expand=accessPackageAssignmentPolicies`.</span><span class="sxs-lookup"><span data-stu-id="6265f-120">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="6265f-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6265f-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6265f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6265f-122">Request headers</span></span>

| <span data-ttu-id="6265f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6265f-123">Name</span></span>      |<span data-ttu-id="6265f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6265f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6265f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6265f-125">Authorization</span></span> | <span data-ttu-id="6265f-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="6265f-126">Bearer \{token\}.</span></span> <span data-ttu-id="6265f-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="6265f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6265f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6265f-128">Request body</span></span>

<span data-ttu-id="6265f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6265f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6265f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6265f-130">Response</span></span>

<span data-ttu-id="6265f-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккаже](../resources/accesspackage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6265f-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6265f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="6265f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6265f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6265f-133">Request</span></span>

<span data-ttu-id="6265f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6265f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```

### <a name="response"></a><span data-ttu-id="6265f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6265f-135">Response</span></span>

<span data-ttu-id="6265f-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6265f-136">The following is an example of the response.</span></span>

> <span data-ttu-id="6265f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6265f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->