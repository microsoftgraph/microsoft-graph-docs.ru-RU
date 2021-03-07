---
title: Удаление печатиTaskTrigger
description: Удаление триггера задач принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e5b4a12e052c3eba729918c40a91ed39542bceb8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517434"
---
# <a name="delete-printtasktrigger"></a><span data-ttu-id="325d2-103">Удаление печатиTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="325d2-103">Delete printTaskTrigger</span></span>
<span data-ttu-id="325d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="325d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="325d2-105">Удалите [триггер задач](../resources/printtasktrigger.md) [принтера, чтобы](../resources/printer.md) предотвратить связанные события печати для запуска задач на указанном принтере.</span><span class="sxs-lookup"><span data-stu-id="325d2-105">Delete the [task trigger](../resources/printtasktrigger.md) of a [printer](../resources/printer.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="325d2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="325d2-106">Permissions</span></span>
<span data-ttu-id="325d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="325d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="325d2-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="325d2-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="325d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="325d2-110">Permission type</span></span> | <span data-ttu-id="325d2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="325d2-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="325d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="325d2-112">Delegated (work or school account)</span></span>| <span data-ttu-id="325d2-113">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="325d2-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="325d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="325d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="325d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="325d2-115">Not Supported.</span></span>|
|<span data-ttu-id="325d2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="325d2-116">Application</span></span>|<span data-ttu-id="325d2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="325d2-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="325d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="325d2-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

## <a name="request-headers"></a><span data-ttu-id="325d2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="325d2-119">Request headers</span></span>
|<span data-ttu-id="325d2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="325d2-120">Name</span></span>|<span data-ttu-id="325d2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="325d2-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="325d2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="325d2-122">Authorization</span></span>|<span data-ttu-id="325d2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="325d2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="325d2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="325d2-125">Request body</span></span>
<span data-ttu-id="325d2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="325d2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="325d2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="325d2-127">Response</span></span>

<span data-ttu-id="325d2-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="325d2-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="325d2-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="325d2-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="325d2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="325d2-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printtasktrigger"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}
```

### <a name="response"></a><span data-ttu-id="325d2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="325d2-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

