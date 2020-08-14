---
title: Список Алловедусерс для принтера
description: Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9cbe7e0c352ab24ccf66283db3c3fd4e1e4dd354
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673751"
---
# <a name="list-allowedusers-for-printer"></a><span data-ttu-id="b41bd-103">Список Алловедусерс для принтера</span><span class="sxs-lookup"><span data-stu-id="b41bd-103">List allowedUsers for printer</span></span>

<span data-ttu-id="b41bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b41bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b41bd-105">Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="b41bd-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b41bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b41bd-106">Permissions</span></span>
<span data-ttu-id="b41bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b41bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b41bd-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b41bd-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="b41bd-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="b41bd-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="b41bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b41bd-111">Permission type</span></span> | <span data-ttu-id="b41bd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b41bd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b41bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b41bd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b41bd-114">Printer. Read. ALL, Printer. ReadWrite. ALL, Printer. FullControl. ALL.</span><span class="sxs-lookup"><span data-stu-id="b41bd-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="b41bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b41bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b41bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b41bd-116">Not Supported.</span></span>|
|<span data-ttu-id="b41bd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b41bd-117">Application</span></span>| <span data-ttu-id="b41bd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b41bd-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b41bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b41bd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b41bd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b41bd-120">Optional query parameters</span></span>
<span data-ttu-id="b41bd-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b41bd-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b41bd-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b41bd-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b41bd-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b41bd-123">Request headers</span></span>
| <span data-ttu-id="b41bd-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b41bd-124">Name</span></span>      |<span data-ttu-id="b41bd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b41bd-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b41bd-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b41bd-126">Authorization</span></span> | <span data-ttu-id="b41bd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b41bd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b41bd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b41bd-129">Request body</span></span>
<span data-ttu-id="b41bd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b41bd-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b41bd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b41bd-131">Response</span></span>
<span data-ttu-id="b41bd-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтусеридентити](../resources/printuseridentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b41bd-132">If successful, this method returns a `200 OK` response code and a collection of [printUserIdentity](../resources/printuseridentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b41bd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b41bd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b41bd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b41bd-134">Request</span></span>
<span data-ttu-id="b41bd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b41bd-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b41bd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b41bd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="b41bd-137">C#</span><span class="sxs-lookup"><span data-stu-id="b41bd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b41bd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b41bd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b41bd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b41bd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b41bd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b41bd-140">Response</span></span>
<span data-ttu-id="b41bd-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b41bd-141">The following is an example of the response.</span></span>
><span data-ttu-id="b41bd-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b41bd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
