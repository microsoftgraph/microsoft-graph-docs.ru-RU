---
title: Список Акцесспаккажересаурцерекуестс
description: Получение списка объектов Акцесспаккажересаурцерекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c9cc83456021c3e10db5fbe1666d7696e8270507
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871902"
---
# <a name="list-accesspackageresourcerequests"></a><span data-ttu-id="66467-103">Список Акцесспаккажересаурцерекуестс</span><span class="sxs-lookup"><span data-stu-id="66467-103">List accessPackageResourceRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66467-104">Получение списка объектов [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="66467-104">Retrieve a list of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="66467-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66467-105">Permissions</span></span>

<span data-ttu-id="66467-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66467-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66467-108">Permission type</span></span>                        | <span data-ttu-id="66467-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66467-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66467-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66467-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="66467-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66467-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="66467-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66467-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66467-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66467-113">Not supported.</span></span> |
| <span data-ttu-id="66467-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66467-114">Application</span></span>                            | <span data-ttu-id="66467-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66467-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66467-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66467-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66467-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66467-117">Optional query parameters</span></span>

<span data-ttu-id="66467-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="66467-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="66467-119">Например, чтобы получить сведения о том, кто запросил Добавление ресурса в каталог, включите `$expand=requestor` в запрос.</span><span class="sxs-lookup"><span data-stu-id="66467-119">For example, to retrieve who requested the addition of a resource to a catalog, include `$expand=requestor` in the query.</span></span> <span data-ttu-id="66467-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="66467-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="66467-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66467-121">Request headers</span></span>

| <span data-ttu-id="66467-122">Имя</span><span class="sxs-lookup"><span data-stu-id="66467-122">Name</span></span>      |<span data-ttu-id="66467-123">Описание</span><span class="sxs-lookup"><span data-stu-id="66467-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="66467-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66467-124">Authorization</span></span> | <span data-ttu-id="66467-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66467-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66467-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66467-127">Request body</span></span>

<span data-ttu-id="66467-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66467-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66467-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="66467-129">Response</span></span>

<span data-ttu-id="66467-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажересаурцерекуест](../resources/accesspackageresourcerequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66467-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66467-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="66467-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66467-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="66467-132">Request</span></span>

<span data-ttu-id="66467-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66467-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerequests"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
```

### <a name="response"></a><span data-ttu-id="66467-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="66467-134">Response</span></span>

<span data-ttu-id="66467-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66467-135">The following is an example of the response.</span></span>

> <span data-ttu-id="66467-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66467-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
      "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
      "isValidationOnly": false,
      "justification": "String",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "requestType": "AdminAdd"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
