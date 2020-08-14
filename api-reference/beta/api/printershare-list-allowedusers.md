---
title: Список Алловедусерс для Принтершаре
description: Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный общий принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: da25944ea966ef6e0326412df6275dd89d1a25d4
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674255"
---
# <a name="list-allowedusers-for-printershare"></a><span data-ttu-id="58486-103">Список Алловедусерс для Принтершаре</span><span class="sxs-lookup"><span data-stu-id="58486-103">List allowedUsers for printerShare</span></span>

<span data-ttu-id="58486-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58486-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58486-105">Получение списка пользователей, которым предоставлен доступ к отправку заданий печати связанному [принтершаре](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="58486-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="58486-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58486-106">Permissions</span></span>
<span data-ttu-id="58486-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="58486-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="58486-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="58486-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="58486-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="58486-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58486-111">Permission type</span></span> | <span data-ttu-id="58486-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58486-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="58486-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58486-113">Delegated (work or school account)</span></span>| <span data-ttu-id="58486-114">Принтершаре. Read. ALL, Принтершаре. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="58486-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="58486-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58486-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58486-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58486-116">Not Supported.</span></span>|
|<span data-ttu-id="58486-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58486-117">Application</span></span>|<span data-ttu-id="58486-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58486-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58486-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58486-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="58486-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58486-120">Request headers</span></span>
| <span data-ttu-id="58486-121">Имя</span><span class="sxs-lookup"><span data-stu-id="58486-121">Name</span></span>      |<span data-ttu-id="58486-122">Описание</span><span class="sxs-lookup"><span data-stu-id="58486-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58486-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58486-123">Authorization</span></span> | <span data-ttu-id="58486-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58486-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58486-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58486-126">Request body</span></span>
<span data-ttu-id="58486-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58486-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="58486-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="58486-128">Response</span></span>
<span data-ttu-id="58486-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтусеридентити](../resources/printuseridentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58486-129">If successful, this method returns a `200 OK` response code and a collection of [printUserIdentity](../resources/printuseridentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="58486-130">Пример</span><span class="sxs-lookup"><span data-stu-id="58486-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="58486-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="58486-131">Request</span></span>
<span data-ttu-id="58486-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58486-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="58486-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="58486-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="58486-134">C#</span><span class="sxs-lookup"><span data-stu-id="58486-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58486-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58486-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58486-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58486-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58486-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="58486-137">Response</span></span>
<span data-ttu-id="58486-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="58486-138">The following is an example of the response.</span></span>
><span data-ttu-id="58486-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58486-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUserIdentity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 286

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printUserIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
