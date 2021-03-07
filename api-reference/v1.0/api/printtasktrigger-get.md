---
title: Получение taskTrigger
description: Получите триггер задачи с принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ab17b71bcdb166b4db2732b88e9ba9b3b4ddc83c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518092"
---
# <a name="get-printtasktrigger"></a><span data-ttu-id="f7cce-103">Get printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="f7cce-103">Get printTaskTrigger</span></span>

<span data-ttu-id="f7cce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7cce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f7cce-105">Получите [триггер задачи](../resources/printtasktrigger.md) с [принтера.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="f7cce-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="f7cce-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="f7cce-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7cce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7cce-107">Permissions</span></span>
<span data-ttu-id="f7cce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f7cce-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="f7cce-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f7cce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7cce-111">Permission type</span></span> | <span data-ttu-id="f7cce-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7cce-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f7cce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7cce-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f7cce-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f7cce-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="f7cce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7cce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7cce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7cce-116">Not Supported.</span></span>|
|<span data-ttu-id="f7cce-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f7cce-117">Application</span></span>|<span data-ttu-id="f7cce-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7cce-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7cce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7cce-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="f7cce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7cce-120">Request headers</span></span>
|<span data-ttu-id="f7cce-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f7cce-121">Name</span></span>|<span data-ttu-id="f7cce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f7cce-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7cce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7cce-123">Authorization</span></span>|<span data-ttu-id="f7cce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7cce-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7cce-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7cce-126">Request body</span></span>
<span data-ttu-id="f7cce-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f7cce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7cce-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7cce-128">Response</span></span>

<span data-ttu-id="f7cce-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект printTaskTrigger](../resources/printtasktrigger.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f7cce-129">If successful, this method returns a `200 OK` response code and a [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7cce-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7cce-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7cce-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7cce-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printtasktrigger"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```


### <a name="response"></a><span data-ttu-id="f7cce-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7cce-132">Response</span></span>
<span data-ttu-id="f7cce-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f7cce-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/taskTriggers/$entity",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

