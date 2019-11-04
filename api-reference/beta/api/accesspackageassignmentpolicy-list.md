---
title: Список АкцесспаккажеассигнментполиЦиес
description: Получение списка объектов Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d2e823980dc9966a5f3e85eef82d00c606e5c180
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936058"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="be2e7-103">Список АкцесспаккажеассигнментполиЦиес</span><span class="sxs-lookup"><span data-stu-id="be2e7-103">List accessPackageAssignmentPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be2e7-104">Получение списка объектов [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в [службе управления обслуживанием Azure AD](../resources/entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="be2e7-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span>   <span data-ttu-id="be2e7-105">Полученный список включает все политики назначения, которые абонент имеет доступ для чтения, во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="be2e7-105">The resulting list includes all the assignment policies which the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="be2e7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be2e7-106">Permissions</span></span>

<span data-ttu-id="be2e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be2e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be2e7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be2e7-109">Permission type</span></span>                        | <span data-ttu-id="be2e7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be2e7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be2e7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be2e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be2e7-112">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="be2e7-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="be2e7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be2e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be2e7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be2e7-114">Not supported.</span></span> |
| <span data-ttu-id="be2e7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be2e7-115">Application</span></span>                            | <span data-ttu-id="be2e7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be2e7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be2e7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be2e7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be2e7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be2e7-118">Optional query parameters</span></span>

<span data-ttu-id="be2e7-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be2e7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="be2e7-120">Например, чтобы получить политику назначения пакетов Access с указанным отображаемым именем, включите `$filter=displayName eq 'Employee sales support'` в запрос.</span><span class="sxs-lookup"><span data-stu-id="be2e7-120">For example, to retrieve a access package assignment policy with a specifed display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="be2e7-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="be2e7-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="be2e7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be2e7-122">Request headers</span></span>

| <span data-ttu-id="be2e7-123">Имя</span><span class="sxs-lookup"><span data-stu-id="be2e7-123">Name</span></span>      |<span data-ttu-id="be2e7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="be2e7-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="be2e7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="be2e7-125">Authorization</span></span> | <span data-ttu-id="be2e7-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="be2e7-126">Bearer \{token\}.</span></span> <span data-ttu-id="be2e7-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="be2e7-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be2e7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be2e7-128">Request body</span></span>

<span data-ttu-id="be2e7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be2e7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be2e7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="be2e7-130">Response</span></span>

<span data-ttu-id="be2e7-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be2e7-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be2e7-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="be2e7-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be2e7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="be2e7-133">Request</span></span>

<span data-ttu-id="be2e7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be2e7-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

### <a name="response"></a><span data-ttu-id="be2e7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="be2e7-135">Response</span></span>

<span data-ttu-id="be2e7-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be2e7-136">The following is an example of the response.</span></span>

> <span data-ttu-id="be2e7-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be2e7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
      "displayName": "All Users",
      "description": "All users can request for access to the directory.",
      "isEnabled": false,
      "canExtend": false,
      "durationInDays": 365
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
