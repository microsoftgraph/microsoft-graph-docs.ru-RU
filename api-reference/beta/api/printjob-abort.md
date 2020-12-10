---
title: 'printJob: Abort'
description: Прервать задание печати.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7a17344dbac7282b12db4b8ebb011f922ceaa01d
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617163"
---
# <a name="printjob-abort"></a><span data-ttu-id="d02a7-103">printJob: Abort</span><span class="sxs-lookup"><span data-stu-id="d02a7-103">printJob: abort</span></span>

<span data-ttu-id="d02a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d02a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d02a7-105">Прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="d02a7-105">Abort a print job.</span></span> <span data-ttu-id="d02a7-106">Только приложения, использующие разрешения приложения, могут прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="d02a7-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="d02a7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d02a7-107">Permissions</span></span>
<span data-ttu-id="d02a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d02a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d02a7-110">В дополнение к следующим разрешениям клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) .</span><span class="sxs-lookup"><span data-stu-id="d02a7-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="d02a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d02a7-111">Permission type</span></span> | <span data-ttu-id="d02a7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d02a7-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d02a7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d02a7-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d02a7-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d02a7-114">Not Supported</span></span> |
|<span data-ttu-id="d02a7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d02a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d02a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d02a7-116">Not Supported.</span></span>|
|<span data-ttu-id="d02a7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d02a7-117">Application</span></span>| <span data-ttu-id="d02a7-118">PrintJob. Реадвритебасик. ALL, PrintJob. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d02a7-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d02a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d02a7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/abort
```
## <a name="request-headers"></a><span data-ttu-id="d02a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d02a7-120">Request headers</span></span>
| <span data-ttu-id="d02a7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d02a7-121">Name</span></span>          | <span data-ttu-id="d02a7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d02a7-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d02a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d02a7-123">Authorization</span></span> | <span data-ttu-id="d02a7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d02a7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d02a7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d02a7-126">Request body</span></span>
<span data-ttu-id="d02a7-127">В тексте запроса можно дополнительно указать причину прерывания задания.</span><span class="sxs-lookup"><span data-stu-id="d02a7-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="d02a7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d02a7-128">Property</span></span>     | <span data-ttu-id="d02a7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d02a7-129">Type</span></span>        | <span data-ttu-id="d02a7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d02a7-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d02a7-131">reason</span><span class="sxs-lookup"><span data-stu-id="d02a7-131">reason</span></span>|<span data-ttu-id="d02a7-132">String</span><span class="sxs-lookup"><span data-stu-id="d02a7-132">String</span></span>|<span data-ttu-id="d02a7-133">Причина аварийного завершения задания.</span><span class="sxs-lookup"><span data-stu-id="d02a7-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="d02a7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d02a7-134">Response</span></span>
<span data-ttu-id="d02a7-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d02a7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d02a7-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d02a7-137">Example</span></span>
<span data-ttu-id="d02a7-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d02a7-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="d02a7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d02a7-139">Request</span></span>
<span data-ttu-id="d02a7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d02a7-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printjob-abort"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/abort
```

### <a name="response"></a><span data-ttu-id="d02a7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d02a7-141">Response</span></span>
<span data-ttu-id="d02a7-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d02a7-142">The following is an example of the response.</span></span> 
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
