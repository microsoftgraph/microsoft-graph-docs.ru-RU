---
title: 'printJob: Канцелпринтжоб'
description: Отмена задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 311236ed0c34064291db93731c5ad8bb62c242a3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035473"
---
# <a name="printjob-cancelprintjob"></a><span data-ttu-id="306fb-103">printJob: Канцелпринтжоб</span><span class="sxs-lookup"><span data-stu-id="306fb-103">printJob: cancelPrintJob</span></span>

<span data-ttu-id="306fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="306fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="306fb-105">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="306fb-105">Cancel a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="306fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="306fb-106">Permissions</span></span>
<span data-ttu-id="306fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="306fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="306fb-109">В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="306fb-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="306fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="306fb-110">Permission type</span></span> | <span data-ttu-id="306fb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="306fb-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="306fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="306fb-112">Delegated (work or school account)</span></span>| <span data-ttu-id="306fb-113">PrintJob. Реадвритебасик, PrintJob. ReadWrite, PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="306fb-113">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="306fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="306fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="306fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="306fb-115">Not Supported.</span></span>|
|<span data-ttu-id="306fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="306fb-116">Application</span></span>| <span data-ttu-id="306fb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="306fb-117">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="306fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="306fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancelPrintJob
```
## <a name="request-headers"></a><span data-ttu-id="306fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="306fb-119">Request headers</span></span>
| <span data-ttu-id="306fb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="306fb-120">Name</span></span>          | <span data-ttu-id="306fb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="306fb-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="306fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="306fb-122">Authorization</span></span> | <span data-ttu-id="306fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="306fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="306fb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="306fb-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="306fb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="306fb-126">Response</span></span>
<span data-ttu-id="306fb-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="306fb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="306fb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="306fb-129">Example</span></span>
<span data-ttu-id="306fb-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="306fb-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="306fb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="306fb-131">Request</span></span>
<span data-ttu-id="306fb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="306fb-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="306fb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="306fb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancelprintjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancelPrintJob
```
# <a name="c"></a>[<span data-ttu-id="306fb-134">C#</span><span class="sxs-lookup"><span data-stu-id="306fb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancelprintjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="306fb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="306fb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancelprintjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="306fb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="306fb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancelprintjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="306fb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="306fb-137">Response</span></span>
<span data-ttu-id="306fb-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="306fb-138">The following is an example of the response.</span></span> 
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
  "description": "printJob: cancelPrintJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


