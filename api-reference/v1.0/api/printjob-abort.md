---
title: 'printJob: прекращение'
description: Прервать задание печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 55ee53dd758116edd14149a9dc20270fa49b1679
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771409"
---
# <a name="printjob-abort"></a><span data-ttu-id="eea45-103">printJob: прекращение</span><span class="sxs-lookup"><span data-stu-id="eea45-103">printJob: abort</span></span>

<span data-ttu-id="eea45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eea45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="eea45-105">Прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="eea45-105">Abort a print job.</span></span> <span data-ttu-id="eea45-106">Только приложения с разрешениями приложений могут прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="eea45-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="eea45-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eea45-107">Permissions</span></span>
<span data-ttu-id="eea45-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eea45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="eea45-110">Помимо следующих разрешений, клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение printer.Read.All или Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="eea45-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="eea45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eea45-111">Permission type</span></span> | <span data-ttu-id="eea45-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eea45-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="eea45-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eea45-113">Delegated (work or school account)</span></span>| <span data-ttu-id="eea45-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eea45-114">Not Supported</span></span> |
|<span data-ttu-id="eea45-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eea45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eea45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eea45-116">Not Supported.</span></span>|
|<span data-ttu-id="eea45-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eea45-117">Application</span></span>| <span data-ttu-id="eea45-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="eea45-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eea45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eea45-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/abort
```

## <a name="request-headers"></a><span data-ttu-id="eea45-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eea45-120">Request headers</span></span>
|<span data-ttu-id="eea45-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eea45-121">Name</span></span>|<span data-ttu-id="eea45-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eea45-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eea45-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eea45-123">Authorization</span></span>|<span data-ttu-id="eea45-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eea45-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eea45-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eea45-126">Request body</span></span>
<span data-ttu-id="eea45-127">В теле запроса можно дополнительно упросить причину, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="eea45-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="eea45-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="eea45-128">Property</span></span>     | <span data-ttu-id="eea45-129">Тип</span><span class="sxs-lookup"><span data-stu-id="eea45-129">Type</span></span>        | <span data-ttu-id="eea45-130">Описание</span><span class="sxs-lookup"><span data-stu-id="eea45-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eea45-131">reason</span><span class="sxs-lookup"><span data-stu-id="eea45-131">reason</span></span>|<span data-ttu-id="eea45-132">String</span><span class="sxs-lookup"><span data-stu-id="eea45-132">String</span></span>|<span data-ttu-id="eea45-133">Причина, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="eea45-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="eea45-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="eea45-134">Response</span></span>

<span data-ttu-id="eea45-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eea45-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eea45-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="eea45-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eea45-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="eea45-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eea45-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="eea45-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_abort"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/abort
Content-Type: application/json
Content-length: 26

{
  "reason": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="eea45-140">C#</span><span class="sxs-lookup"><span data-stu-id="eea45-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eea45-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eea45-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eea45-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eea45-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eea45-143">Java</span><span class="sxs-lookup"><span data-stu-id="eea45-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eea45-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="eea45-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

