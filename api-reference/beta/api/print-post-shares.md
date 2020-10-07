---
title: Создание printerShare
description: Создает новую общую папку принтера для указанного принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 53752d7a6f0b703334c85582397066fa1a52f7bc
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373933"
---
# <a name="create-printershare"></a><span data-ttu-id="dcf93-103">Создание printerShare</span><span class="sxs-lookup"><span data-stu-id="dcf93-103">Create printerShare</span></span>

<span data-ttu-id="dcf93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcf93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf93-105">Создание нового **принтершаре** для указанного [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="dcf93-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf93-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcf93-106">Permissions</span></span>
<span data-ttu-id="dcf93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcf93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dcf93-109">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать в дополнение к разрешениям, приведенным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="dcf93-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="dcf93-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="dcf93-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="dcf93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcf93-111">Permission type</span></span> | <span data-ttu-id="dcf93-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcf93-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="dcf93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcf93-113">Delegated (work or school account)</span></span>| <span data-ttu-id="dcf93-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcf93-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="dcf93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcf93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcf93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcf93-116">Not Supported.</span></span>|
|<span data-ttu-id="dcf93-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="dcf93-117">Application</span></span>|<span data-ttu-id="dcf93-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcf93-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcf93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcf93-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares
```
## <a name="request-headers"></a><span data-ttu-id="dcf93-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcf93-120">Request headers</span></span>
| <span data-ttu-id="dcf93-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dcf93-121">Name</span></span>          | <span data-ttu-id="dcf93-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dcf93-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dcf93-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcf93-123">Authorization</span></span> | <span data-ttu-id="dcf93-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcf93-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcf93-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dcf93-126">Content-type</span></span>  | <span data-ttu-id="dcf93-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcf93-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcf93-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dcf93-129">Request body</span></span>
<span data-ttu-id="dcf93-130">В тексте запроса добавьте представление объекта [принтершаре](../resources/printershare.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcf93-130">In the request body, supply a JSON representation of [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="dcf93-131">Свойства **ID** и **createdDateTime** для общего ресурса принтера задаются автоматически при создании ресурса, но имя общего ресурса и связанный принтер должны быть включены в запрос.</span><span class="sxs-lookup"><span data-stu-id="dcf93-131">The printer share's **id** and **createdDateTime** properties are set automatically upon resource creation, but the share name and associated printer must be included in the request.</span></span>

<span data-ttu-id="dcf93-132">Ссылка принтера задается с помощью `@odata.bind` синтаксиса, как показано в примере.</span><span class="sxs-lookup"><span data-stu-id="dcf93-132">The printer reference is set by using `@odata.bind` syntax, as shown in the example.</span></span>

## <a name="response"></a><span data-ttu-id="dcf93-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcf93-133">Response</span></span>
<span data-ttu-id="dcf93-134">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dcf93-134">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcf93-135">Пример</span><span class="sxs-lookup"><span data-stu-id="dcf93-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcf93-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcf93-136">Request</span></span>
<span data-ttu-id="dcf93-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcf93-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcf93-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf93-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_print"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares
Content-type: application/json
Content-length: 114

{
  "name": "name-value",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="dcf93-139">C#</span><span class="sxs-lookup"><span data-stu-id="dcf93-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printershare-from-print-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcf93-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcf93-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printershare-from-print-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcf93-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcf93-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printershare-from-print-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dcf93-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcf93-142">Response</span></span>
<span data-ttu-id="dcf93-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcf93-143">The following is an example of the response.</span></span>
><span data-ttu-id="dcf93-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcf93-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 233

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
    "id": "7361c7c1-ff07-4565-9897-bef6895a7d04",
    "name": "ShareName",
    "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
