---
title: Список разрешенных Групп для принтераShare
description: Извлечение списка групп, которые получили доступ для отправки заданий печати в связанную долю принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 49555364c6ff923d746718ef37650130d85e7c30
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771570"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="6b22d-103">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="6b22d-103">List allowedGroups</span></span>
<span data-ttu-id="6b22d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b22d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="6b22d-105">Извлечение списка групп, которые получили доступ для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="6b22d-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b22d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b22d-106">Permissions</span></span>
<span data-ttu-id="6b22d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b22d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6b22d-109">Помимо следующих разрешений, клиент пользователя или приложения должен иметь активную подписку на универсальную печать и иметь разрешение, да которое предоставляет доступ [к группам](group-list.md) списков.</span><span class="sxs-lookup"><span data-stu-id="6b22d-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List groups](group-list.md) access.</span></span> <span data-ttu-id="6b22d-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="6b22d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="6b22d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b22d-111">Permission type</span></span> | <span data-ttu-id="6b22d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b22d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6b22d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b22d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6b22d-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b22d-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="6b22d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b22d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b22d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b22d-116">Not Supported.</span></span>|
|<span data-ttu-id="6b22d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b22d-117">Application</span></span>|<span data-ttu-id="6b22d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b22d-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b22d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b22d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="6b22d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b22d-120">Request headers</span></span>
|<span data-ttu-id="6b22d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6b22d-121">Name</span></span>|<span data-ttu-id="6b22d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6b22d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6b22d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b22d-123">Authorization</span></span>|<span data-ttu-id="6b22d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b22d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b22d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b22d-126">Request body</span></span>
<span data-ttu-id="6b22d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b22d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b22d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b22d-128">Response</span></span>

<span data-ttu-id="6b22d-129">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="6b22d-129">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b22d-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b22d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6b22d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b22d-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6b22d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b22d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="6b22d-133">C#</span><span class="sxs-lookup"><span data-stu-id="6b22d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b22d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b22d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b22d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b22d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b22d-136">Java</span><span class="sxs-lookup"><span data-stu-id="6b22d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6b22d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b22d-137">Response</span></span>
<span data-ttu-id="6b22d-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b22d-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.group)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "GroupName"
    }
  ]
}
```

