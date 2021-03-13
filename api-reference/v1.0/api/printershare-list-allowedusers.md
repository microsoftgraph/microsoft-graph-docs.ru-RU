---
title: Список allowedUsers для printerShare
description: Извлечение списка пользователей, которым был предоставлен доступ для отправки заданий печати в связанную долю принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: d1f55d9d4ae91d6ae41ee4656fbb1e90b7948304
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771535"
---
# <a name="list-allowedusers"></a><span data-ttu-id="dba83-103">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="dba83-103">List allowedUsers</span></span>
<span data-ttu-id="dba83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dba83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="dba83-105">Извлечение списка пользователей, которым был предоставлен доступ для отправки заданий печати в связанный [принтерShare.](../resources/printershare.md)</span><span class="sxs-lookup"><span data-stu-id="dba83-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dba83-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dba83-106">Permissions</span></span>
<span data-ttu-id="dba83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dba83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dba83-109">Помимо следующих разрешений, клиент или клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение, да которое предоставляет [доступ пользователям списка.](user-list.md)</span><span class="sxs-lookup"><span data-stu-id="dba83-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List users](user-list.md) access.</span></span> <span data-ttu-id="dba83-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="dba83-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="dba83-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dba83-111">Permission type</span></span> | <span data-ttu-id="dba83-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dba83-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="dba83-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dba83-113">Delegated (work or school account)</span></span>| <span data-ttu-id="dba83-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba83-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="dba83-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dba83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dba83-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dba83-116">Not Supported.</span></span>|
|<span data-ttu-id="dba83-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dba83-117">Application</span></span>|<span data-ttu-id="dba83-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dba83-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dba83-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dba83-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="dba83-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dba83-120">Request headers</span></span>
|<span data-ttu-id="dba83-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dba83-121">Name</span></span>|<span data-ttu-id="dba83-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dba83-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dba83-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dba83-123">Authorization</span></span>|<span data-ttu-id="dba83-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dba83-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dba83-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dba83-126">Request body</span></span>
<span data-ttu-id="dba83-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dba83-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dba83-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dba83-128">Response</span></span>

<span data-ttu-id="dba83-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dba83-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dba83-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="dba83-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dba83-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dba83-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dba83-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dba83-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_user"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="dba83-133">C#</span><span class="sxs-lookup"><span data-stu-id="dba83-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dba83-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dba83-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dba83-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dba83-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dba83-136">Java</span><span class="sxs-lookup"><span data-stu-id="dba83-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dba83-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dba83-137">Response</span></span>
<span data-ttu-id="dba83-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dba83-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.user)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.user)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@contoso.com"
    }
  ]
}
```

