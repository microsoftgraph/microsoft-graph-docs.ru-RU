---
title: Обновление конфигурации printJob
description: Обновление конфигурации задания печати
author: tomsato-ms
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1f4d2f1c5573e7f4ad4ae150c598788ab40163ab
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843591"
---
# <a name="update-printjob-configuration"></a><span data-ttu-id="8e645-103">Обновление конфигурации printJob</span><span class="sxs-lookup"><span data-stu-id="8e645-103">Update printJob configuration</span></span>

<span data-ttu-id="8e645-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e645-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e645-105">Обновление свойства [конфигурации](../resources/printjobconfiguration.md) задания [печати.](../resources/printjob.md)</span><span class="sxs-lookup"><span data-stu-id="8e645-105">Update the [configuration](../resources/printjobconfiguration.md) property of a [print job](../resources/printjob.md).</span></span>

<span data-ttu-id="8e645-106">Обновление конфигурации задания печати будет успешным, только если для связанного задания печати есть состояние [printTask,](../resources/printTask.md) запущенный триггером, запрашивающий `processing` приложение.</span><span class="sxs-lookup"><span data-stu-id="8e645-106">Updating a print job configuration will only succeed if there is a [printTask](../resources/printTask.md) in `processing` state on the associated print job, started by a trigger that requesting app created.</span></span> <span data-ttu-id="8e645-107">Подробные сведения о регистрации триггера задачи см. в подзадаче "Расширение универсальной печати [для поддержки печати с потягивом".](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="8e645-107">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e645-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e645-108">Permissions</span></span>
<span data-ttu-id="8e645-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e645-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8e645-111">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть активная подписка на универсальную печать, разрешение printer.Read.All или Printer.ReadWrite.All, а также одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8e645-111">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="8e645-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e645-112">Permission type</span></span> | <span data-ttu-id="8e645-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e645-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8e645-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e645-114">Delegated (work or school account)</span></span>| <span data-ttu-id="8e645-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e645-115">Not supported.</span></span> |
|<span data-ttu-id="8e645-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e645-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e645-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e645-117">Not Supported.</span></span>|
|<span data-ttu-id="8e645-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e645-118">Application</span></span>| <span data-ttu-id="8e645-119">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e645-119">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e645-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e645-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}/configuration
```
## <a name="request-headers"></a><span data-ttu-id="8e645-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e645-121">Request headers</span></span>
| <span data-ttu-id="8e645-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8e645-122">Name</span></span>          | <span data-ttu-id="8e645-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8e645-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e645-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e645-124">Authorization</span></span> | <span data-ttu-id="8e645-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e645-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e645-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e645-127">Request body</span></span>
<span data-ttu-id="8e645-128">В теле запроса укажийте значения соответствующих полей [printJobConfiguration.](../resources/printjobconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e645-128">In the request body, supply the values of the relevant [printJobConfiguration](../resources/printjobconfiguration.md) fields.</span></span> <span data-ttu-id="8e645-129">Существующие свойства, не включенные в тело запроса, сохраняют свои прежние значения.</span><span class="sxs-lookup"><span data-stu-id="8e645-129">Existing properties that are not included in the request body will maintain their previous values.</span></span>

## <a name="response"></a><span data-ttu-id="8e645-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e645-130">Response</span></span>
<span data-ttu-id="8e645-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8e645-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8e645-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8e645-132">Example</span></span>
<span data-ttu-id="8e645-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8e645-133">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="8e645-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e645-134">Request</span></span>
<span data-ttu-id="8e645-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e645-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e645-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e645-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-update-configuration"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration

{
  "feedOrientation": "longEdgeFirst",
  "pageRanges": [
    {
      "start": 1,
      "end": 1
    }
  ],
  "quality": "medium",
  "dpi": 600,
  "orientation": "landscape",
  "copies": 1,
  "duplexMode": "oneSided",
  "colorMode": "blackAndWhite",
  "inputBin": "by-pass-tray",
  "outputBin": "output-tray",
  "mediaSize": "A4",
  "margin": {
    "top": 0,
    "bottom": 0,
    "left": 0,
    "right": 0
  },
  "mediaType": "stationery",
  "finishings": null,
  "pagesPerSheet": 1,
  "multipageLayout": "clockwiseFromBottomLeft",
  "collate": false,
  "scaling": "shrinkToFit",
  "fitPdfToPage": false
}
```
# <a name="c"></a>[<span data-ttu-id="8e645-137">C#</span><span class="sxs-lookup"><span data-stu-id="8e645-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-update-configuration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e645-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e645-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-update-configuration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e645-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e645-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-update-configuration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e645-140">Java</span><span class="sxs-lookup"><span data-stu-id="8e645-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-update-configuration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="8e645-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e645-141">Response</span></span>
<span data-ttu-id="8e645-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e645-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update print job configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


