---
title: 'printJob: redirect'
description: Перенаправление задания печати на другой принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3564997c25cb41a94a83780bd3dca5f04a92ca9c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091666"
---
# <a name="printjob-redirect"></a><span data-ttu-id="e487f-103">printJob: redirect</span><span class="sxs-lookup"><span data-stu-id="e487f-103">printJob: redirect</span></span>

<span data-ttu-id="e487f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e487f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e487f-105">Перенаправление [задания печати](../resources/printjob.md) на другой [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="e487f-105">Redirect a [print job](../resources/printjob.md) to a different [printer](../resources/printer.md).</span></span>

<span data-ttu-id="e487f-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="e487f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="e487f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e487f-107">Permissions</span></span>
<span data-ttu-id="e487f-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e487f-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e487f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e487f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e487f-110">Чтобы использовать универсальную службу печати, пользователь или клиент приложения должен иметь активную универсальную подписку на печать, разрешение, предоставляющее доступ к [принтеру](printer-get.md) , а также одно из разрешений, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e487f-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="e487f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e487f-111">Permission type</span></span> | <span data-ttu-id="e487f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e487f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e487f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e487f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e487f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e487f-114">Not supported.</span></span> |
|<span data-ttu-id="e487f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e487f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e487f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e487f-116">Not Supported.</span></span>|
|<span data-ttu-id="e487f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e487f-117">Application</span></span>| <span data-ttu-id="e487f-118">PrintJob. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="e487f-118">PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e487f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e487f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/redirect
```
## <a name="request-headers"></a><span data-ttu-id="e487f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e487f-120">Request headers</span></span>
| <span data-ttu-id="e487f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e487f-121">Name</span></span>          | <span data-ttu-id="e487f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e487f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e487f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e487f-123">Authorization</span></span> | <span data-ttu-id="e487f-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e487f-124">Bearer {token}.</span></span> <span data-ttu-id="e487f-125">Required.</span><span class="sxs-lookup"><span data-stu-id="e487f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e487f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e487f-126">Request body</span></span>
<span data-ttu-id="e487f-127">В тексте запроса укажите идентификатор принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="e487f-127">In the request body, supply the ID of the printer that the print job should be redirected to.</span></span>

| <span data-ttu-id="e487f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e487f-128">Property</span></span>     | <span data-ttu-id="e487f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e487f-129">Type</span></span>        | <span data-ttu-id="e487f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e487f-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e487f-131">дестинатионпринтерид</span><span class="sxs-lookup"><span data-stu-id="e487f-131">destinationPrinterId</span></span>|<span data-ttu-id="e487f-132">String</span><span class="sxs-lookup"><span data-stu-id="e487f-132">String</span></span>|<span data-ttu-id="e487f-133">ИДЕНТИФИКАТОР принтера, на который необходимо перенаправить задание печати.</span><span class="sxs-lookup"><span data-stu-id="e487f-133">The ID of the printer the print job should be redirected to.</span></span>|

## <a name="response"></a><span data-ttu-id="e487f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e487f-134">Response</span></span>
<span data-ttu-id="e487f-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [printJob](../resources/printjob.md) , помещенные в очередь для конечного принтера.</span><span class="sxs-lookup"><span data-stu-id="e487f-135">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object queued for the destination printer.</span></span>

## <a name="example"></a><span data-ttu-id="e487f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e487f-136">Example</span></span>
<span data-ttu-id="e487f-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e487f-137">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="e487f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e487f-138">Request</span></span>
<span data-ttu-id="e487f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e487f-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printjob-redirect"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/redirect

{
  "destinationPrinterId": "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea"
}
```

---

### <a name="response"></a><span data-ttu-id="e487f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e487f-140">Response</span></span>
<span data-ttu-id="e487f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e487f-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 437

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#printJob",
  "@odata.type": "#microsoft.graph.printJob",
  "id": "44354",
  "createdDateTime": "2020-06-30T17:19:09Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed by the printer."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: redirect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
