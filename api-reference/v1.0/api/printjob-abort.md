---
title: 'printJob: прекращение'
description: Прервать задание печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 4f9bfb7623e546c402853c31eba750f5c4040966
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080094"
---
# <a name="printjob-abort"></a><span data-ttu-id="357e7-103">printJob: прекращение</span><span class="sxs-lookup"><span data-stu-id="357e7-103">printJob: abort</span></span>

<span data-ttu-id="357e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="357e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="357e7-105">Прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="357e7-105">Abort a print job.</span></span> <span data-ttu-id="357e7-106">Только приложения с разрешениями приложений могут прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="357e7-106">Only applications using application permissions can abort a print job.</span></span>

<span data-ttu-id="357e7-107">Прерывание задания печати будет успешным только в том случае, если в связанной работе печати имеется [printTask,](../resources/printTask.md) запущенный с триггера, созданного приложением-запросом. `processing`</span><span class="sxs-lookup"><span data-stu-id="357e7-107">Aborting a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="357e7-108">Подробные сведения о регистрации триггера задач см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="357e7-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="357e7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="357e7-109">Permissions</span></span>
<span data-ttu-id="357e7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="357e7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="357e7-112">Помимо следующих разрешений, клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение printer.Read.All или Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="357e7-112">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="357e7-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="357e7-113">Permission type</span></span> | <span data-ttu-id="357e7-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="357e7-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="357e7-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="357e7-115">Delegated (work or school account)</span></span>| <span data-ttu-id="357e7-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="357e7-116">Not Supported</span></span> |
|<span data-ttu-id="357e7-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="357e7-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="357e7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="357e7-118">Not Supported.</span></span>|
|<span data-ttu-id="357e7-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="357e7-119">Application</span></span>| <span data-ttu-id="357e7-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="357e7-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="357e7-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="357e7-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/abort
```

## <a name="request-headers"></a><span data-ttu-id="357e7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="357e7-122">Request headers</span></span>
|<span data-ttu-id="357e7-123">Имя</span><span class="sxs-lookup"><span data-stu-id="357e7-123">Name</span></span>|<span data-ttu-id="357e7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="357e7-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="357e7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="357e7-125">Authorization</span></span>|<span data-ttu-id="357e7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="357e7-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="357e7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="357e7-128">Request body</span></span>
<span data-ttu-id="357e7-129">В теле запроса можно дополнительно упросить причину, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="357e7-129">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="357e7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="357e7-130">Property</span></span>     | <span data-ttu-id="357e7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="357e7-131">Type</span></span>        | <span data-ttu-id="357e7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="357e7-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="357e7-133">reason</span><span class="sxs-lookup"><span data-stu-id="357e7-133">reason</span></span>|<span data-ttu-id="357e7-134">String</span><span class="sxs-lookup"><span data-stu-id="357e7-134">String</span></span>|<span data-ttu-id="357e7-135">Причина, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="357e7-135">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="357e7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="357e7-136">Response</span></span>

<span data-ttu-id="357e7-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="357e7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="357e7-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="357e7-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="357e7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="357e7-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="357e7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="357e7-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="357e7-142">C#</span><span class="sxs-lookup"><span data-stu-id="357e7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="357e7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="357e7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="357e7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="357e7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="357e7-145">Java</span><span class="sxs-lookup"><span data-stu-id="357e7-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="357e7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="357e7-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

