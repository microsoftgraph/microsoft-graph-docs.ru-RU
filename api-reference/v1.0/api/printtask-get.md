---
title: Вывод задачи
description: Сведения о задаче печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0aff8e70271a0903289a50eb4fb76b21d9269cab
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517415"
---
# <a name="get-printtask"></a><span data-ttu-id="42e63-103">Get printTask</span><span class="sxs-lookup"><span data-stu-id="42e63-103">Get printTask</span></span>
<span data-ttu-id="42e63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42e63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="42e63-105">Сведения о задаче печати.</span><span class="sxs-lookup"><span data-stu-id="42e63-105">Get details about a print task.</span></span>

<span data-ttu-id="42e63-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="42e63-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="42e63-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42e63-107">Permissions</span></span>
<span data-ttu-id="42e63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42e63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="42e63-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="42e63-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="42e63-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42e63-111">Permission type</span></span> | <span data-ttu-id="42e63-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42e63-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="42e63-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42e63-113">Delegated (work or school account)</span></span>| <span data-ttu-id="42e63-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42e63-114">Not supported.</span></span> |
|<span data-ttu-id="42e63-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42e63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42e63-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42e63-116">Not Supported.</span></span>|
|<span data-ttu-id="42e63-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="42e63-117">Application</span></span>| <span data-ttu-id="42e63-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42e63-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42e63-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42e63-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="42e63-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42e63-120">Request headers</span></span>
|<span data-ttu-id="42e63-121">Имя</span><span class="sxs-lookup"><span data-stu-id="42e63-121">Name</span></span>|<span data-ttu-id="42e63-122">Описание</span><span class="sxs-lookup"><span data-stu-id="42e63-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="42e63-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42e63-123">Authorization</span></span>|<span data-ttu-id="42e63-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42e63-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="42e63-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42e63-126">Request body</span></span>
<span data-ttu-id="42e63-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42e63-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42e63-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="42e63-128">Response</span></span>

<span data-ttu-id="42e63-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printTask](../resources/printtask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="42e63-129">If successful, this method returns a `200 OK` response code and a [printTask](../resources/printtask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42e63-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="42e63-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42e63-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="42e63-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printtask"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}
```

### <a name="response"></a><span data-ttu-id="42e63-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="42e63-132">Response</span></span>
<span data-ttu-id="42e63-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="42e63-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions('3203656e-6069-4e10-8147-d25290b00a3c')/tasks/$entity",
  "id": "d036638b-1272-4bba-9227-732463823ed3",
  "parentUrl": "https://graph.microsoft.com/v1.0/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353",
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```

