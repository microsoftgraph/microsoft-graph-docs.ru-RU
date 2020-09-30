---
title: Список Алловедграупс для принтера
description: Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 98989c3c672e3353bc4a80b62d7365827e6a452f
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315579"
---
# <a name="list-allowedgroups-for-printer"></a><span data-ttu-id="b6463-103">Список Алловедграупс для принтера</span><span class="sxs-lookup"><span data-stu-id="b6463-103">List allowedGroups for printer</span></span>

<span data-ttu-id="b6463-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6463-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6463-105">Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="b6463-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6463-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6463-106">Permissions</span></span>
<span data-ttu-id="b6463-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6463-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b6463-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="b6463-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="b6463-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="b6463-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="b6463-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6463-111">Permission type</span></span> | <span data-ttu-id="b6463-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6463-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b6463-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6463-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b6463-114">Printer. Read. ALL, Printer. ReadWrite. ALL, Printer. FullControl. ALL.</span><span class="sxs-lookup"><span data-stu-id="b6463-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="b6463-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6463-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6463-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6463-116">Not Supported.</span></span>|
|<span data-ttu-id="b6463-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6463-117">Application</span></span>| <span data-ttu-id="b6463-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6463-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6463-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6463-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6463-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b6463-120">Optional query parameters</span></span>
<span data-ttu-id="b6463-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b6463-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b6463-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b6463-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6463-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6463-123">Request headers</span></span>
| <span data-ttu-id="b6463-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b6463-124">Name</span></span>      |<span data-ttu-id="b6463-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b6463-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6463-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6463-126">Authorization</span></span> | <span data-ttu-id="b6463-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6463-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6463-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6463-129">Request body</span></span>
<span data-ttu-id="b6463-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6463-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b6463-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6463-131">Response</span></span>
<span data-ttu-id="b6463-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтидентити](../resources/printidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6463-132">If successful, this method returns a `200 OK` response code and a collection of [printIdentity](../resources/printidentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6463-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b6463-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6463-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6463-134">Request</span></span>
<span data-ttu-id="b6463-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6463-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6463-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6463-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="b6463-137">C#</span><span class="sxs-lookup"><span data-stu-id="b6463-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6463-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6463-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6463-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6463-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b6463-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6463-140">Response</span></span>
<span data-ttu-id="b6463-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6463-141">The following is an example of the response.</span></span>
><span data-ttu-id="b6463-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6463-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printIdentity",
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