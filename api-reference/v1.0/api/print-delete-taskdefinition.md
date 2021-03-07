---
title: Удаление taskDefinition
description: Удаление определения задачи.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 457ebc3ba3f2e125b5d252c138ed08b28d3e0798
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517385"
---
# <a name="delete-printtaskdefinition"></a><span data-ttu-id="5f39f-103">Удаление печатиTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5f39f-103">Delete printTaskDefinition</span></span>
<span data-ttu-id="5f39f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f39f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5f39f-105">Удаление **taskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="5f39f-105">Delete a **taskDefinition**.</span></span>

<span data-ttu-id="5f39f-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="5f39f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f39f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f39f-107">Permissions</span></span>
<span data-ttu-id="5f39f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f39f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5f39f-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="5f39f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="5f39f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f39f-111">Permission type</span></span> | <span data-ttu-id="5f39f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f39f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5f39f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f39f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5f39f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f39f-114">Not supported.</span></span> |
|<span data-ttu-id="5f39f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f39f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f39f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f39f-116">Not Supported.</span></span>|
|<span data-ttu-id="5f39f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5f39f-117">Application</span></span>| <span data-ttu-id="5f39f-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f39f-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f39f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f39f-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="5f39f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f39f-120">Request headers</span></span>
|<span data-ttu-id="5f39f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5f39f-121">Name</span></span>|<span data-ttu-id="5f39f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5f39f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f39f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f39f-123">Authorization</span></span>|<span data-ttu-id="5f39f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f39f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f39f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f39f-126">Request body</span></span>
<span data-ttu-id="5f39f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f39f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f39f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f39f-128">Response</span></span>
<span data-ttu-id="5f39f-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5f39f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f39f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f39f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f39f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f39f-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printtaskdefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```


### <a name="response"></a><span data-ttu-id="5f39f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f39f-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

