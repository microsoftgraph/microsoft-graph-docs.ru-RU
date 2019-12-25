---
title: Получение Акцесспаккажеассигнментресаурцероле
description: Получение свойств и связей объекта Акцесспаккажеассигнментресаурцероле.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a3d7cc1beaaadaf37da83045b9ab270022f8e32e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871907"
---
# <a name="get-accesspackageassignmentresourcerole"></a><span data-ttu-id="e0b88-103">Получение Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="e0b88-103">Get accessPackageAssignmentResourceRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0b88-104">Получение свойств и связей объекта [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="e0b88-104">Retrieve the properties and relationships of an [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0b88-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0b88-105">Permissions</span></span>

<span data-ttu-id="e0b88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0b88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0b88-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0b88-108">Permission type</span></span>                        | <span data-ttu-id="e0b88-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0b88-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0b88-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0b88-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0b88-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b88-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="e0b88-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0b88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0b88-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0b88-113">Not supported.</span></span> |
| <span data-ttu-id="e0b88-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0b88-114">Application</span></span>                            | <span data-ttu-id="e0b88-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0b88-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0b88-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0b88-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0b88-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e0b88-117">Optional query parameters</span></span>

<span data-ttu-id="e0b88-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e0b88-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e0b88-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e0b88-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0b88-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0b88-120">Request headers</span></span>

| <span data-ttu-id="e0b88-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e0b88-121">Name</span></span>      |<span data-ttu-id="e0b88-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e0b88-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0b88-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0b88-123">Authorization</span></span> | <span data-ttu-id="e0b88-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0b88-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0b88-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0b88-126">Request body</span></span>

<span data-ttu-id="e0b88-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0b88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0b88-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0b88-128">Response</span></span>

<span data-ttu-id="e0b88-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажеассигнментресаурцероле](../resources/accesspackageassignmentresourcerole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0b88-129">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0b88-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e0b88-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0b88-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0b88-131">Request</span></span>

<span data-ttu-id="e0b88-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0b88-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourcerole"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}
```

### <a name="response"></a><span data-ttu-id="e0b88-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0b88-133">Response</span></span>

<span data-ttu-id="e0b88-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e0b88-134">The following is an example of the response.</span></span>

> <span data-ttu-id="e0b88-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0b88-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
  "originId": "originId-value",
  "originSystem": "SharePointOnline",
  "status": "Fulfilled"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentResourceRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
