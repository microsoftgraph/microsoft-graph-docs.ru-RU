---
title: 'printJob: отмена'
description: Отмена задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b2eb7c40f1f2474752b316a412dbb4c382152741
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787515"
---
# <a name="printjob-cancel"></a><span data-ttu-id="f4897-103">printJob: отмена</span><span class="sxs-lookup"><span data-stu-id="f4897-103">printJob: cancel</span></span>

<span data-ttu-id="f4897-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4897-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4897-105">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="f4897-105">Cancel a print job.</span></span> <span data-ttu-id="f4897-106">Задания печати можно отменить только от имени пользователя с помощью делегирования разрешений.</span><span class="sxs-lookup"><span data-stu-id="f4897-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4897-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4897-107">Permissions</span></span>
<span data-ttu-id="f4897-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4897-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f4897-110">Помимо следующих разрешений, пользователь или клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет [доступ к принтеру Get.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="f4897-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="f4897-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4897-111">Permission type</span></span> | <span data-ttu-id="f4897-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4897-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f4897-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4897-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f4897-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4897-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="f4897-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4897-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4897-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4897-116">Not Supported.</span></span>|
|<span data-ttu-id="f4897-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f4897-117">Application</span></span>| <span data-ttu-id="f4897-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4897-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4897-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4897-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/cancel
```
## <a name="request-headers"></a><span data-ttu-id="f4897-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4897-120">Request headers</span></span>
| <span data-ttu-id="f4897-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f4897-121">Name</span></span>          | <span data-ttu-id="f4897-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f4897-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f4897-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4897-123">Authorization</span></span> | <span data-ttu-id="f4897-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4897-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4897-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4897-126">Request body</span></span>
<span data-ttu-id="f4897-127">Тело запроса должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="f4897-127">Request body should be empty.</span></span>

## <a name="response"></a><span data-ttu-id="f4897-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4897-128">Response</span></span>
<span data-ttu-id="f4897-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f4897-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4897-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f4897-131">Example</span></span>
<span data-ttu-id="f4897-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f4897-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="f4897-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4897-133">Request</span></span>
<span data-ttu-id="f4897-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4897-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f4897-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4897-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-cancel"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/cancel
```
# <a name="c"></a>[<span data-ttu-id="f4897-136">C#</span><span class="sxs-lookup"><span data-stu-id="f4897-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4897-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4897-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4897-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4897-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4897-139">Java</span><span class="sxs-lookup"><span data-stu-id="f4897-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4897-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4897-140">Response</span></span>
<span data-ttu-id="f4897-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f4897-141">The following is an example of the response.</span></span> 
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
  "description": "printJob: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


