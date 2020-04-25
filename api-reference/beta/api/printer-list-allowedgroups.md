---
title: Список allowedGroups
description: Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 22943f9ffaaee83922d9ecaca41b6307c56ea97e
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812510"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="07c7d-103">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="07c7d-103">List allowedGroups</span></span>

<span data-ttu-id="07c7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07c7d-105">Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="07c7d-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="07c7d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07c7d-106">Permissions</span></span>
<span data-ttu-id="07c7d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="07c7d-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="07c7d-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="07c7d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07c7d-110">Permission type</span></span> | <span data-ttu-id="07c7d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07c7d-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="07c7d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07c7d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="07c7d-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="07c7d-113">Users.Read.All</span></span> |
|<span data-ttu-id="07c7d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07c7d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07c7d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c7d-115">Not Supported.</span></span>|
|<span data-ttu-id="07c7d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07c7d-116">Application</span></span>|<span data-ttu-id="07c7d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c7d-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c7d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07c7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07c7d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07c7d-119">Optional query parameters</span></span>
<span data-ttu-id="07c7d-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07c7d-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="07c7d-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="07c7d-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="07c7d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07c7d-122">Request headers</span></span>
| <span data-ttu-id="07c7d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="07c7d-123">Name</span></span>      |<span data-ttu-id="07c7d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="07c7d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07c7d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07c7d-125">Authorization</span></span> | <span data-ttu-id="07c7d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07c7d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07c7d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07c7d-128">Request body</span></span>
<span data-ttu-id="07c7d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07c7d-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="07c7d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="07c7d-130">Response</span></span>
<span data-ttu-id="07c7d-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Identity](../resources/identity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07c7d-131">If successful, this method returns a `200 OK` response code and a collection of [identity](../resources/identity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07c7d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="07c7d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07c7d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="07c7d-133">Request</span></span>
<span data-ttu-id="07c7d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07c7d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07c7d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="07c7d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="07c7d-136">C#</span><span class="sxs-lookup"><span data-stu-id="07c7d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07c7d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07c7d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07c7d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07c7d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07c7d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="07c7d-139">Response</span></span>
<span data-ttu-id="07c7d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07c7d-140">The following is an example of the response.</span></span>
><span data-ttu-id="07c7d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07c7d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "GroupName"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
