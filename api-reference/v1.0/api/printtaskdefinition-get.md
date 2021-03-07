---
title: Get taskDefinition
description: Сведения об определении задачи.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 88f892d511514ecd02e6b8ab10372dfa4de7a2b1
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517331"
---
# <a name="get-printtaskdefinition"></a><span data-ttu-id="d2165-103">Get printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="d2165-103">Get printTaskDefinition</span></span>

<span data-ttu-id="d2165-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2165-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d2165-105">Сведения об определении задачи.</span><span class="sxs-lookup"><span data-stu-id="d2165-105">Get details about a task definition.</span></span>

<span data-ttu-id="d2165-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="d2165-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2165-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2165-107">Permissions</span></span>
<span data-ttu-id="d2165-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d2165-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="d2165-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d2165-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2165-111">Permission type</span></span> | <span data-ttu-id="d2165-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2165-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d2165-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2165-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d2165-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2165-114">Not supported.</span></span> |
|<span data-ttu-id="d2165-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2165-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2165-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2165-116">Not Supported.</span></span>|
|<span data-ttu-id="d2165-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2165-117">Application</span></span>| <span data-ttu-id="d2165-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2165-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2165-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2165-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="d2165-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2165-120">Request headers</span></span>
|<span data-ttu-id="d2165-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d2165-121">Name</span></span>|<span data-ttu-id="d2165-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d2165-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2165-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2165-123">Authorization</span></span>|<span data-ttu-id="d2165-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2165-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2165-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2165-126">Request body</span></span>
<span data-ttu-id="d2165-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2165-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2165-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2165-128">Response</span></span>

<span data-ttu-id="d2165-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2165-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2165-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2165-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2165-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2165-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printtaskdefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```

### <a name="response"></a><span data-ttu-id="d2165-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2165-132">Response</span></span>
<span data-ttu-id="d2165-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d2165-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

