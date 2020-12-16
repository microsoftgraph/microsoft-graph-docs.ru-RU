---
title: 'printJob: abort'
description: Отменить задание печати.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8fe447b11a8198af41bf9e69e98a7ea64231dec8
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691112"
---
# <a name="printjob-abort"></a><span data-ttu-id="d879a-103">printJob: abort</span><span class="sxs-lookup"><span data-stu-id="d879a-103">printJob: abort</span></span>

<span data-ttu-id="d879a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d879a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d879a-105">Отменить задание печати.</span><span class="sxs-lookup"><span data-stu-id="d879a-105">Abort a print job.</span></span> <span data-ttu-id="d879a-106">Только приложения, использующие разрешения приложений, могут отменить задание печати.</span><span class="sxs-lookup"><span data-stu-id="d879a-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="d879a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d879a-107">Permissions</span></span>
<span data-ttu-id="d879a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d879a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d879a-110">Помимо перечисленных ниже разрешений, клиент приложения должен иметь активную подписку универсальной печати и разрешение, которое предоставляет доступ [к принтеру.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="d879a-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="d879a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d879a-111">Permission type</span></span> | <span data-ttu-id="d879a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d879a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d879a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d879a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d879a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d879a-114">Not Supported</span></span> |
|<span data-ttu-id="d879a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d879a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d879a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d879a-116">Not Supported.</span></span>|
|<span data-ttu-id="d879a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d879a-117">Application</span></span>| <span data-ttu-id="d879a-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d879a-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d879a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d879a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/abort
```
## <a name="request-headers"></a><span data-ttu-id="d879a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d879a-120">Request headers</span></span>
| <span data-ttu-id="d879a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d879a-121">Name</span></span>          | <span data-ttu-id="d879a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d879a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d879a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d879a-123">Authorization</span></span> | <span data-ttu-id="d879a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d879a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d879a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d879a-126">Request body</span></span>
<span data-ttu-id="d879a-127">При желании в теле запроса можно упросить причину, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="d879a-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="d879a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d879a-128">Property</span></span>     | <span data-ttu-id="d879a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d879a-129">Type</span></span>        | <span data-ttu-id="d879a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d879a-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d879a-131">reason</span><span class="sxs-lookup"><span data-stu-id="d879a-131">reason</span></span>|<span data-ttu-id="d879a-132">String</span><span class="sxs-lookup"><span data-stu-id="d879a-132">String</span></span>|<span data-ttu-id="d879a-133">Причина, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="d879a-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="d879a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d879a-134">Response</span></span>
<span data-ttu-id="d879a-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d879a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d879a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d879a-137">Example</span></span>
<span data-ttu-id="d879a-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d879a-138">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="d879a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d879a-139">Request</span></span>
<span data-ttu-id="d879a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d879a-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d879a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="d879a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-abort"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/abort
```
# <a name="c"></a>[<span data-ttu-id="d879a-142">C#</span><span class="sxs-lookup"><span data-stu-id="d879a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-abort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d879a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d879a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-abort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d879a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d879a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-abort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d879a-145">Java</span><span class="sxs-lookup"><span data-stu-id="d879a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-abort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d879a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d879a-146">Response</span></span>
<span data-ttu-id="d879a-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d879a-147">The following is an example of the response.</span></span> 
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
