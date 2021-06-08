---
title: 'printJob: прекращение'
description: Прервать задание печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 6aa15af9b316012b777c641e6e23bbcc1e463071
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787396"
---
# <a name="printjob-abort"></a><span data-ttu-id="6e51f-103">printJob: прекращение</span><span class="sxs-lookup"><span data-stu-id="6e51f-103">printJob: abort</span></span>

<span data-ttu-id="6e51f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e51f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e51f-105">Прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="6e51f-105">Abort a print job.</span></span> <span data-ttu-id="6e51f-106">Только приложения с разрешениями приложений могут прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="6e51f-106">Only applications using application permissions can abort a print job.</span></span>

<span data-ttu-id="6e51f-107">Прерывание задания печати будет успешным только в том случае, если в связанной работе печати имеется [printTask,](../resources/printTask.md) запущенный с триггера, созданного приложением-запросом. `processing`</span><span class="sxs-lookup"><span data-stu-id="6e51f-107">Aborting a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="6e51f-108">Подробные сведения о регистрации триггера задач см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="6e51f-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e51f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e51f-109">Permissions</span></span>
<span data-ttu-id="6e51f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e51f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6e51f-112">Помимо следующих разрешений, клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение printer.Read.All или Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="6e51f-112">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="6e51f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e51f-113">Permission type</span></span> | <span data-ttu-id="6e51f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e51f-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6e51f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e51f-115">Delegated (work or school account)</span></span>| <span data-ttu-id="6e51f-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6e51f-116">Not Supported</span></span> |
|<span data-ttu-id="6e51f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e51f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e51f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e51f-118">Not Supported.</span></span>|
|<span data-ttu-id="6e51f-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="6e51f-119">Application</span></span>| <span data-ttu-id="6e51f-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="6e51f-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e51f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e51f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/abort
```
## <a name="request-headers"></a><span data-ttu-id="6e51f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e51f-122">Request headers</span></span>
| <span data-ttu-id="6e51f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6e51f-123">Name</span></span>          | <span data-ttu-id="6e51f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6e51f-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6e51f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e51f-125">Authorization</span></span> | <span data-ttu-id="6e51f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e51f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e51f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e51f-128">Request body</span></span>
<span data-ttu-id="6e51f-129">В теле запроса можно дополнительно упросить причину, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="6e51f-129">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="6e51f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e51f-130">Property</span></span>     | <span data-ttu-id="6e51f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6e51f-131">Type</span></span>        | <span data-ttu-id="6e51f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6e51f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e51f-133">reason</span><span class="sxs-lookup"><span data-stu-id="6e51f-133">reason</span></span>|<span data-ttu-id="6e51f-134">String</span><span class="sxs-lookup"><span data-stu-id="6e51f-134">String</span></span>|<span data-ttu-id="6e51f-135">Причина, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="6e51f-135">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="6e51f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e51f-136">Response</span></span>
<span data-ttu-id="6e51f-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6e51f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e51f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6e51f-139">Example</span></span>
<span data-ttu-id="6e51f-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6e51f-140">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="6e51f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e51f-141">Request</span></span>
<span data-ttu-id="6e51f-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e51f-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e51f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e51f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-abort"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/abort
```
# <a name="c"></a>[<span data-ttu-id="6e51f-144">C#</span><span class="sxs-lookup"><span data-stu-id="6e51f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e51f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e51f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e51f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e51f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e51f-147">Java</span><span class="sxs-lookup"><span data-stu-id="6e51f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e51f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e51f-148">Response</span></span>
<span data-ttu-id="6e51f-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6e51f-149">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
