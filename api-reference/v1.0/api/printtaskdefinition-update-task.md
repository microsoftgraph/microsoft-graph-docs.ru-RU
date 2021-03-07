---
title: Обновление задачи
description: Обновление задачи печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 684d2063f069b3e7444e0727c2b2d9ad14fe7113
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518033"
---
# <a name="update-printtask"></a><span data-ttu-id="9cd6a-103">Обновление printTask</span><span class="sxs-lookup"><span data-stu-id="9cd6a-103">Update printTask</span></span>
<span data-ttu-id="9cd6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cd6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="9cd6a-105">Обновление задачи печати.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-105">Update a print task.</span></span>

<span data-ttu-id="9cd6a-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="9cd6a-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="9cd6a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cd6a-107">Permissions</span></span>
<span data-ttu-id="9cd6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cd6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9cd6a-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="9cd6a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cd6a-111">Permission type</span></span> | <span data-ttu-id="9cd6a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cd6a-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9cd6a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cd6a-113">Delegated (work or school account)</span></span>| <span data-ttu-id="9cd6a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-114">Not supported.</span></span> |
|<span data-ttu-id="9cd6a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cd6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cd6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-116">Not Supported.</span></span>|
|<span data-ttu-id="9cd6a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9cd6a-117">Application</span></span>| <span data-ttu-id="9cd6a-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cd6a-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cd6a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cd6a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="9cd6a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cd6a-120">Request headers</span></span>
|<span data-ttu-id="9cd6a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9cd6a-121">Name</span></span>|<span data-ttu-id="9cd6a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9cd6a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9cd6a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cd6a-123">Authorization</span></span>|<span data-ttu-id="9cd6a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9cd6a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cd6a-126">Content-Type</span></span>|<span data-ttu-id="9cd6a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cd6a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cd6a-129">Request body</span></span>

<span data-ttu-id="9cd6a-130">В теле запроса укажи значения для соответствующих полей [printTask,](../resources/printtask.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-130">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="9cd6a-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9cd6a-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9cd6a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cd6a-133">Property</span></span>     | <span data-ttu-id="9cd6a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9cd6a-134">Type</span></span>        | <span data-ttu-id="9cd6a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9cd6a-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9cd6a-136">status</span><span class="sxs-lookup"><span data-stu-id="9cd6a-136">status</span></span>|<span data-ttu-id="9cd6a-137">String</span><span class="sxs-lookup"><span data-stu-id="9cd6a-137">String</span></span>|<span data-ttu-id="9cd6a-138">`state` `description` Включай и значения, описывая текущее состояние задачи.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-138">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="9cd6a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cd6a-139">Response</span></span>

<span data-ttu-id="9cd6a-140">В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект printTask](../resources/printtask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-140">If successful, this method returns a `200 OK` response code and an updated [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9cd6a-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="9cd6a-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9cd6a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cd6a-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printtask"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
Content-Type: application/json
Content-length: 152

{
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```

### <a name="response"></a><span data-ttu-id="9cd6a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cd6a-143">Response</span></span>
<span data-ttu-id="9cd6a-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9cd6a-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "Task execution is completed."
  }
}
```

