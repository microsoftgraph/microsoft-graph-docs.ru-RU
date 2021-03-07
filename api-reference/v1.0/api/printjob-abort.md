---
title: 'printJob: прекращение'
description: Прервать задание печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f179b30e7c07d9f577ab63c59142a68362a389f1
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518109"
---
# <a name="printjob-abort"></a><span data-ttu-id="13ff6-103">printJob: прекращение</span><span class="sxs-lookup"><span data-stu-id="13ff6-103">printJob: abort</span></span>

<span data-ttu-id="13ff6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13ff6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="13ff6-105">Прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="13ff6-105">Abort a print job.</span></span> <span data-ttu-id="13ff6-106">Только приложения с разрешениями приложений могут прервать задание печати.</span><span class="sxs-lookup"><span data-stu-id="13ff6-106">Only applications using application permissions can abort a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="13ff6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13ff6-107">Permissions</span></span>
<span data-ttu-id="13ff6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13ff6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="13ff6-110">Помимо следующих разрешений, клиент приложения должен иметь активную подписку на универсальную печать и иметь разрешение printer.Read.All или Printer.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="13ff6-110">In addition to the following permissions, the app's tenant must have an active Universal Print subscription and have either the Printer.Read.All or Printer.ReadWrite.All application permission.</span></span>

|<span data-ttu-id="13ff6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13ff6-111">Permission type</span></span> | <span data-ttu-id="13ff6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13ff6-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="13ff6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13ff6-113">Delegated (work or school account)</span></span>| <span data-ttu-id="13ff6-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="13ff6-114">Not Supported</span></span> |
|<span data-ttu-id="13ff6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13ff6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13ff6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13ff6-116">Not Supported.</span></span>|
|<span data-ttu-id="13ff6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="13ff6-117">Application</span></span>| <span data-ttu-id="13ff6-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="13ff6-118">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13ff6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13ff6-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/abort
```

## <a name="request-headers"></a><span data-ttu-id="13ff6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13ff6-120">Request headers</span></span>
|<span data-ttu-id="13ff6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="13ff6-121">Name</span></span>|<span data-ttu-id="13ff6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="13ff6-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="13ff6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13ff6-123">Authorization</span></span>|<span data-ttu-id="13ff6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13ff6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="13ff6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13ff6-126">Request body</span></span>
<span data-ttu-id="13ff6-127">В теле запроса можно дополнительно упросить причину, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="13ff6-127">In the request body, you can optionally provide the reason why the job is being aborted.</span></span>

| <span data-ttu-id="13ff6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="13ff6-128">Property</span></span>     | <span data-ttu-id="13ff6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="13ff6-129">Type</span></span>        | <span data-ttu-id="13ff6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="13ff6-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13ff6-131">reason</span><span class="sxs-lookup"><span data-stu-id="13ff6-131">reason</span></span>|<span data-ttu-id="13ff6-132">Строка</span><span class="sxs-lookup"><span data-stu-id="13ff6-132">String</span></span>|<span data-ttu-id="13ff6-133">Причина, по которой задание прерывается.</span><span class="sxs-lookup"><span data-stu-id="13ff6-133">Reason why job is being aborted.</span></span>|

## <a name="response"></a><span data-ttu-id="13ff6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="13ff6-134">Response</span></span>

<span data-ttu-id="13ff6-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13ff6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13ff6-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="13ff6-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13ff6-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="13ff6-138">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="13ff6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="13ff6-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

