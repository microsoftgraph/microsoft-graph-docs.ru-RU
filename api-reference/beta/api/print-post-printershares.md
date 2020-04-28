---
title: Создание Принтершаре
description: Создает новую общую папку принтера для указанного принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8846f43b61e370260571174313d4c2a07adf4cec
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948235"
---
# <a name="create-printershare"></a><span data-ttu-id="94969-103">Создание Принтершаре</span><span class="sxs-lookup"><span data-stu-id="94969-103">Create printerShare</span></span>

<span data-ttu-id="94969-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94969-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94969-105">Создание нового **принтершаре** для указанного [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="94969-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94969-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94969-106">Permissions</span></span>
<span data-ttu-id="94969-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="94969-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="94969-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="94969-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94969-110">Permission type</span></span> | <span data-ttu-id="94969-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94969-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="94969-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94969-112">Delegated (work or school account)</span></span>| <span data-ttu-id="94969-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="94969-113">Users.Read.All</span></span> |
|<span data-ttu-id="94969-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94969-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94969-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94969-115">Not Supported.</span></span>|
|<span data-ttu-id="94969-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94969-116">Application</span></span>|<span data-ttu-id="94969-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94969-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94969-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94969-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printerShares
```
## <a name="request-headers"></a><span data-ttu-id="94969-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94969-119">Request headers</span></span>
| <span data-ttu-id="94969-120">Имя</span><span class="sxs-lookup"><span data-stu-id="94969-120">Name</span></span>          | <span data-ttu-id="94969-121">Описание</span><span class="sxs-lookup"><span data-stu-id="94969-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="94969-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94969-122">Authorization</span></span> | <span data-ttu-id="94969-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94969-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94969-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94969-125">Content-type</span></span>  | <span data-ttu-id="94969-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94969-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94969-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="94969-128">Request body</span></span>
<span data-ttu-id="94969-129">В тексте запроса добавьте представление объекта [принтершаре](../resources/printershare.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94969-129">In the request body, supply a JSON representation of [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="94969-130">Свойства **ID** и **createdDateTime** для общего ресурса принтера задаются автоматически при создании ресурса, но имя общего ресурса и связанный принтер должны быть включены в запрос.</span><span class="sxs-lookup"><span data-stu-id="94969-130">The printer share's **id** and **createdDateTime** properties are set automatically upon resource creation, but the share name and associated printer must be included in the request.</span></span>

<span data-ttu-id="94969-131">Ссылка принтера задается с помощью `@odata.bind` синтаксиса, как показано в примере.</span><span class="sxs-lookup"><span data-stu-id="94969-131">The printer reference is set by using `@odata.bind` syntax, as shown in the example.</span></span>

## <a name="response"></a><span data-ttu-id="94969-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="94969-132">Response</span></span>
<span data-ttu-id="94969-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94969-133">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94969-134">Пример</span><span class="sxs-lookup"><span data-stu-id="94969-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94969-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="94969-135">Request</span></span>
<span data-ttu-id="94969-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94969-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94969-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="94969-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_print"
}-->
```http
POST https://graph.microsoft.com/beta/print/printerShares
Content-type: application/json
Content-length: 114

{
  "name": "name-value",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="94969-138">C#</span><span class="sxs-lookup"><span data-stu-id="94969-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printershare-from-print-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94969-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94969-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printershare-from-print-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94969-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94969-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printershare-from-print-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94969-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="94969-141">Response</span></span>
<span data-ttu-id="94969-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="94969-142">The following is an example of the response.</span></span>
><span data-ttu-id="94969-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94969-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares/$entity",
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
