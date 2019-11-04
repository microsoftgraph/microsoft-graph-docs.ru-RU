---
title: Список Акцесспаккажересаурцес
description: Получение списка объектов акцесспаккажересаурце.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ebb1d6ce33c2f10da19162d40f097c1043af62e8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936086"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="6913a-103">Список Акцесспаккажересаурцес</span><span class="sxs-lookup"><span data-stu-id="6913a-103">List accessPackageResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6913a-104">Получение списка объектов [акцесспаккажересаурце](../resources/accesspackageresource.md) в [акцесспаккажекаталог](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="6913a-104">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6913a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6913a-105">Permissions</span></span>

<span data-ttu-id="6913a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6913a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6913a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6913a-108">Permission type</span></span>                        | <span data-ttu-id="6913a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6913a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6913a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6913a-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="6913a-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6913a-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6913a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6913a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6913a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6913a-113">Not supported.</span></span> |
| <span data-ttu-id="6913a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6913a-114">Application</span></span>                            | <span data-ttu-id="6913a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6913a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6913a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6913a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6913a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6913a-117">Optional query parameters</span></span>

<span data-ttu-id="6913a-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6913a-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6913a-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6913a-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6913a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6913a-120">Request headers</span></span>

| <span data-ttu-id="6913a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6913a-121">Name</span></span>      |<span data-ttu-id="6913a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6913a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6913a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6913a-123">Authorization</span></span> | <span data-ttu-id="6913a-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="6913a-124">Bearer \{token\}.</span></span> <span data-ttu-id="6913a-125">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="6913a-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6913a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6913a-126">Request body</span></span>

<span data-ttu-id="6913a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6913a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6913a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6913a-128">Response</span></span>

<span data-ttu-id="6913a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажересаурце](../resources/accesspackageresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6913a-129">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6913a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="6913a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6913a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6913a-131">Request</span></span>

<span data-ttu-id="6913a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6913a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

### <a name="response"></a><span data-ttu-id="6913a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6913a-133">Response</span></span>

<span data-ttu-id="6913a-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6913a-134">The following is an example of the response.</span></span>

> <span data-ttu-id="6913a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6913a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
