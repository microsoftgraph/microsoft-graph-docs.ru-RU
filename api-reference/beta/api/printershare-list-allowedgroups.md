---
title: Список разрешенных Групп для принтераShare
description: Извлечение списка групп, которые получили доступ для отправки заданий печати в связанную долю принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0a15472fd7935dc3eacc38c0a34a6e7a5c0eaf67
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766275"
---
# <a name="list-allowedgroups-for-printershare"></a><span data-ttu-id="84c34-103">Список разрешенных Групп для принтераShare</span><span class="sxs-lookup"><span data-stu-id="84c34-103">List allowedGroups for printerShare</span></span>

<span data-ttu-id="84c34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84c34-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84c34-105">Извлечение списка групп, которые получили доступ для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="84c34-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="84c34-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84c34-106">Permissions</span></span>
<span data-ttu-id="84c34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84c34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="84c34-109">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, да которое предоставляет доступ [к группам](group-list.md) списков.</span><span class="sxs-lookup"><span data-stu-id="84c34-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List groups](group-list.md) access.</span></span> <span data-ttu-id="84c34-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="84c34-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="84c34-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84c34-111">Permission type</span></span> | <span data-ttu-id="84c34-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84c34-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="84c34-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84c34-113">Delegated (work or school account)</span></span>| <span data-ttu-id="84c34-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84c34-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="84c34-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84c34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84c34-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84c34-116">Not Supported.</span></span>|
|<span data-ttu-id="84c34-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="84c34-117">Application</span></span>|<span data-ttu-id="84c34-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84c34-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84c34-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84c34-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="84c34-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84c34-120">Request headers</span></span>
| <span data-ttu-id="84c34-121">Имя</span><span class="sxs-lookup"><span data-stu-id="84c34-121">Name</span></span>      |<span data-ttu-id="84c34-122">Описание</span><span class="sxs-lookup"><span data-stu-id="84c34-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84c34-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84c34-123">Authorization</span></span> | <span data-ttu-id="84c34-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84c34-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84c34-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84c34-126">Request body</span></span>
<span data-ttu-id="84c34-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84c34-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="84c34-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="84c34-128">Response</span></span>
<span data-ttu-id="84c34-129">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="84c34-129">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84c34-130">Пример</span><span class="sxs-lookup"><span data-stu-id="84c34-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84c34-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="84c34-131">Request</span></span>
<span data-ttu-id="84c34-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84c34-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="84c34-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="84c34-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="84c34-134">C#</span><span class="sxs-lookup"><span data-stu-id="84c34-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84c34-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84c34-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84c34-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84c34-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84c34-137">Java</span><span class="sxs-lookup"><span data-stu-id="84c34-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allowedgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84c34-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="84c34-138">Response</span></span>
<span data-ttu-id="84c34-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84c34-139">The following is an example of the response.</span></span>
><span data-ttu-id="84c34-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84c34-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 233

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.group)",
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
