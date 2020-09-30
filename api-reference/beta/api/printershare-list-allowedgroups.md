---
title: Список Алловедграупс для Принтершаре
description: Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный общий принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 0f964a1964ed7ec676563c676337ecdb85b48498
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314829"
---
# <a name="list-allowedgroups-for-printershare"></a><span data-ttu-id="c25c0-103">Список Алловедграупс для Принтершаре</span><span class="sxs-lookup"><span data-stu-id="c25c0-103">List allowedGroups for printerShare</span></span>

<span data-ttu-id="c25c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c25c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c25c0-105">Получение списка групп, которым предоставлен доступ к отправку заданий печати связанному [принтершаре](../resources/printershare.md).</span><span class="sxs-lookup"><span data-stu-id="c25c0-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c25c0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c25c0-106">Permissions</span></span>
<span data-ttu-id="c25c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c25c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c25c0-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c25c0-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="c25c0-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="c25c0-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c25c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c25c0-111">Permission type</span></span> | <span data-ttu-id="c25c0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c25c0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c25c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c25c0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c25c0-114">Принтершаре. Read. ALL, Принтершаре. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c25c0-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="c25c0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c25c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c25c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c25c0-116">Not Supported.</span></span>|
|<span data-ttu-id="c25c0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c25c0-117">Application</span></span>|<span data-ttu-id="c25c0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c25c0-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c25c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c25c0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="c25c0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c25c0-120">Request headers</span></span>
| <span data-ttu-id="c25c0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c25c0-121">Name</span></span>      |<span data-ttu-id="c25c0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c25c0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c25c0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c25c0-123">Authorization</span></span> | <span data-ttu-id="c25c0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c25c0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c25c0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c25c0-126">Request body</span></span>
<span data-ttu-id="c25c0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c25c0-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c25c0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c25c0-128">Response</span></span>
<span data-ttu-id="c25c0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принтидентити](../resources/printidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c25c0-129">If successful, this method returns a `200 OK` response code and a collection of [printIdentity](../resources/printidentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c25c0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c25c0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c25c0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c25c0-131">Request</span></span>
<span data-ttu-id="c25c0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c25c0-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c25c0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c25c0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedGroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="c25c0-134">C#</span><span class="sxs-lookup"><span data-stu-id="c25c0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c25c0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c25c0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c25c0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c25c0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c25c0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c25c0-137">Response</span></span>
<span data-ttu-id="c25c0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c25c0-138">The following is an example of the response.</span></span>
><span data-ttu-id="c25c0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c25c0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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