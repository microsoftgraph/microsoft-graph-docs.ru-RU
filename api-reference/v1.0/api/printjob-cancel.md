---
title: 'printJob: отмена'
description: Отмена задания печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dd341ddc3beff0ece8ba28e1071f217f9cac05ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777056"
---
# <a name="printjob-cancel"></a><span data-ttu-id="b9394-103">printJob: отмена</span><span class="sxs-lookup"><span data-stu-id="b9394-103">printJob: cancel</span></span>
<span data-ttu-id="b9394-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9394-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b9394-105">Отмена задания печати.</span><span class="sxs-lookup"><span data-stu-id="b9394-105">Cancel a print job.</span></span> <span data-ttu-id="b9394-106">Задания печати можно отменить только от имени пользователя с помощью делегирования разрешений.</span><span class="sxs-lookup"><span data-stu-id="b9394-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9394-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9394-107">Permissions</span></span>
<span data-ttu-id="b9394-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9394-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b9394-110">Помимо следующих разрешений, пользователь или клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение, которое предоставляет [доступ к принтеру Get.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="b9394-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="b9394-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9394-111">Permission type</span></span> | <span data-ttu-id="b9394-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9394-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b9394-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9394-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b9394-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9394-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="b9394-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9394-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9394-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9394-116">Not Supported.</span></span>|
|<span data-ttu-id="b9394-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b9394-117">Application</span></span>| <span data-ttu-id="b9394-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9394-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9394-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9394-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="b9394-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9394-120">Request headers</span></span>
|<span data-ttu-id="b9394-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b9394-121">Name</span></span>|<span data-ttu-id="b9394-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b9394-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9394-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9394-123">Authorization</span></span>|<span data-ttu-id="b9394-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9394-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9394-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9394-126">Request body</span></span>
<span data-ttu-id="b9394-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9394-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9394-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9394-128">Response</span></span>
<span data-ttu-id="b9394-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9394-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9394-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9394-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9394-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9394-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b9394-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9394-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob_cancel"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="b9394-134">C#</span><span class="sxs-lookup"><span data-stu-id="b9394-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9394-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9394-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9394-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9394-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9394-137">Java</span><span class="sxs-lookup"><span data-stu-id="b9394-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9394-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9394-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

