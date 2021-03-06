---
title: 'printJob: прекращение'
description: Прервать задание печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: cfd82c356463f3e642d5817ff0203c2bec8627db
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515452"
---
# <a name="printjob-abort"></a><span data-ttu-id="28122-103">printJob: прекращение</span><span class="sxs-lookup"><span data-stu-id="28122-103">printJob: abort</span></span>

<span data-ttu-id="28122-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28122-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28122-105">Прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="28122-105">Abort a print job.</span></span> <span data-ttu-id="28122-106">Только приложения с разрешениями приложений могут прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="28122-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="28122-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28122-107">Permissions</span></span>
<span data-ttu-id="28122-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28122-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="28122-110">Помимо следующих разрешений, клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение printer.Read.All или Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="28122-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="28122-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28122-111">Permission type</span></span> | <span data-ttu-id="28122-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28122-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="28122-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28122-113">Delegated (work or school account)</span></span>| <span data-ttu-id="28122-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="28122-114">Not Supported</span></span> |
|<span data-ttu-id="28122-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28122-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28122-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28122-116">Not Supported.</span></span>|
|<span data-ttu-id="28122-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28122-117">Application</span></span>| <span data-ttu-id="28122-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="28122-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28122-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28122-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/abort
```
## <a name="request-headers"></a><span data-ttu-id="28122-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28122-120">Request headers</span></span>
| <span data-ttu-id="28122-121">Имя</span><span class="sxs-lookup"><span data-stu-id="28122-121">Name</span></span>          | <span data-ttu-id="28122-122">Описание</span><span class="sxs-lookup"><span data-stu-id="28122-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="28122-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28122-123">Authorization</span></span> | <span data-ttu-id="28122-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28122-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28122-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28122-126">Request body</span></span>
<span data-ttu-id="28122-127">В теле запроса можно дополнительно упросить причину, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="28122-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="28122-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="28122-128">Property</span></span>     | <span data-ttu-id="28122-129">Тип</span><span class="sxs-lookup"><span data-stu-id="28122-129">Type</span></span>        | <span data-ttu-id="28122-130">Описание</span><span class="sxs-lookup"><span data-stu-id="28122-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="28122-131">reason</span><span class="sxs-lookup"><span data-stu-id="28122-131">reason</span></span>|<span data-ttu-id="28122-132">String</span><span class="sxs-lookup"><span data-stu-id="28122-132">String</span></span>|<span data-ttu-id="28122-133">Причина, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="28122-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="28122-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="28122-134">Response</span></span>
<span data-ttu-id="28122-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28122-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28122-137">Пример</span><span class="sxs-lookup"><span data-stu-id="28122-137">Example</span></span>
<span data-ttu-id="28122-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="28122-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="28122-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="28122-139">Request</span></span>
<span data-ttu-id="28122-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28122-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="28122-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="28122-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-abort"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/abort
```
# <a name="c"></a>[<span data-ttu-id="28122-142">C#</span><span class="sxs-lookup"><span data-stu-id="28122-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28122-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28122-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28122-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28122-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28122-145">Java</span><span class="sxs-lookup"><span data-stu-id="28122-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28122-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="28122-146">Response</span></span>
<span data-ttu-id="28122-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28122-147">The following is an example of the response.</span></span> 
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
  "description": "printJob: abort",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
