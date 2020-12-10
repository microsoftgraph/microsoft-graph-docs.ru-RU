---
title: 'printJob: Cancel'
description: Отмена задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4c4522ef8fb19226475758986d1245c447358095
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617019"
---
# <a name="printjob-cancel"></a><span data-ttu-id="4275f-103">printJob: Cancel</span><span class="sxs-lookup"><span data-stu-id="4275f-103">printJob: cancel</span></span>

<span data-ttu-id="4275f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4275f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4275f-105">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="4275f-105">Cancel a print job.</span></span> <span data-ttu-id="4275f-106">Задания печати могут быть отменены только от имени пользователя, используя делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="4275f-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="4275f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4275f-107">Permissions</span></span>
<span data-ttu-id="4275f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4275f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4275f-110">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="4275f-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="4275f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4275f-111">Permission type</span></span> | <span data-ttu-id="4275f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4275f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4275f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4275f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4275f-114">PrintJob. Реадвритебасик, PrintJob. ReadWrite, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4275f-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="4275f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4275f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4275f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4275f-116">Not Supported.</span></span>|
|<span data-ttu-id="4275f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4275f-117">Application</span></span>| <span data-ttu-id="4275f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4275f-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4275f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4275f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="4275f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4275f-120">Request headers</span></span>
| <span data-ttu-id="4275f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4275f-121">Name</span></span>          | <span data-ttu-id="4275f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4275f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4275f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4275f-123">Authorization</span></span> | <span data-ttu-id="4275f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4275f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4275f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4275f-126">Request body</span></span>
<span data-ttu-id="4275f-127">Текст запроса должен быть пустым.</span><span class="sxs-lookup"><span data-stu-id="4275f-127">Request body should be empty.</span></span>

## <a name="response"></a><span data-ttu-id="4275f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4275f-128">Response</span></span>
<span data-ttu-id="4275f-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4275f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4275f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4275f-131">Example</span></span>
<span data-ttu-id="4275f-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4275f-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="4275f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4275f-133">Request</span></span>
<span data-ttu-id="4275f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4275f-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4275f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4275f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancel"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancel
```
# <a name="c"></a>[<span data-ttu-id="4275f-136">C#</span><span class="sxs-lookup"><span data-stu-id="4275f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4275f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4275f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4275f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4275f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4275f-139">Java</span><span class="sxs-lookup"><span data-stu-id="4275f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4275f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4275f-140">Response</span></span>
<span data-ttu-id="4275f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4275f-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


