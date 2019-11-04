---
title: Получение Акцесспаккажеассигнментполици
description: Получение свойств и связей объекта Акцесспаккажеаассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a0b3279188c4650efba4ae73cb7c1fccd4ae57ef
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936063"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="43b03-103">Получение Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="43b03-103">Get accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43b03-104">В разделе [Управление обслуживанием Azure AD](../resources/entitlementmanagement-root.md)извлекаются свойства и связи объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="43b03-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="43b03-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43b03-105">Permissions</span></span>

<span data-ttu-id="43b03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43b03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43b03-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43b03-108">Permission type</span></span>                        | <span data-ttu-id="43b03-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43b03-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="43b03-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43b03-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="43b03-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="43b03-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="43b03-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43b03-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43b03-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43b03-113">Not supported.</span></span> |
| <span data-ttu-id="43b03-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43b03-114">Application</span></span>                            | <span data-ttu-id="43b03-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43b03-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43b03-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43b03-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43b03-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43b03-117">Optional query parameters</span></span>

<span data-ttu-id="43b03-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43b03-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="43b03-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="43b03-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="43b03-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43b03-120">Request headers</span></span>

| <span data-ttu-id="43b03-121">Имя</span><span class="sxs-lookup"><span data-stu-id="43b03-121">Name</span></span>      |<span data-ttu-id="43b03-122">Описание</span><span class="sxs-lookup"><span data-stu-id="43b03-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="43b03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43b03-123">Authorization</span></span> | <span data-ttu-id="43b03-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="43b03-124">Bearer \{token\}.</span></span> <span data-ttu-id="43b03-125">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="43b03-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43b03-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43b03-126">Request body</span></span>

<span data-ttu-id="43b03-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43b03-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43b03-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="43b03-128">Response</span></span>

<span data-ttu-id="43b03-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43b03-129">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43b03-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="43b03-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43b03-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="43b03-131">Request</span></span>

<span data-ttu-id="43b03-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43b03-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="43b03-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="43b03-133">Response</span></span>

<span data-ttu-id="43b03-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="43b03-134">The following is an example of the response.</span></span>

> <span data-ttu-id="43b03-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43b03-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isEnabled": false,
  "canExtend": false,
  "durationInDays": 365
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
