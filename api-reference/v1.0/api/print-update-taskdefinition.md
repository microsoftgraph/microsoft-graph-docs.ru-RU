---
title: Обновление печатиTaskDefinition
description: Обновление определения задачи.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 98f075e89828a1e07fe3ee04bbed0b95b511b0d5
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517499"
---
# <a name="update-printtaskdefinition"></a><span data-ttu-id="300a9-103">Обновление печатиTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="300a9-103">Update printTaskDefinition</span></span>

<span data-ttu-id="300a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="300a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="300a9-105">Обновление определения задачи.</span><span class="sxs-lookup"><span data-stu-id="300a9-105">Update a task definition.</span></span>

<span data-ttu-id="300a9-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="300a9-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="300a9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="300a9-107">Permissions</span></span>
<span data-ttu-id="300a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="300a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="300a9-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="300a9-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="300a9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="300a9-111">Permission type</span></span> | <span data-ttu-id="300a9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="300a9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="300a9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="300a9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="300a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="300a9-114">Not supported.</span></span> |
|<span data-ttu-id="300a9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="300a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="300a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="300a9-116">Not Supported.</span></span>|
|<span data-ttu-id="300a9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="300a9-117">Application</span></span>| <span data-ttu-id="300a9-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="300a9-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="300a9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="300a9-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="300a9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="300a9-120">Request headers</span></span>
|<span data-ttu-id="300a9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="300a9-121">Name</span></span>|<span data-ttu-id="300a9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="300a9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="300a9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="300a9-123">Authorization</span></span>|<span data-ttu-id="300a9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="300a9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="300a9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="300a9-126">Content-Type</span></span>|<span data-ttu-id="300a9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="300a9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="300a9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="300a9-129">Request body</span></span>
<span data-ttu-id="300a9-130">В теле запроса укажи значения для соответствующих полей [printTaskDefinition,](../resources/printtaskdefinition.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="300a9-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="300a9-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="300a9-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="300a9-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="300a9-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="300a9-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="300a9-133">Property</span></span>     | <span data-ttu-id="300a9-134">Тип</span><span class="sxs-lookup"><span data-stu-id="300a9-134">Type</span></span>        | <span data-ttu-id="300a9-135">Описание</span><span class="sxs-lookup"><span data-stu-id="300a9-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="300a9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="300a9-136">displayName</span></span>|<span data-ttu-id="300a9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="300a9-137">String</span></span>|<span data-ttu-id="300a9-138">Имя **печатиTaskDefinition**.</span><span class="sxs-lookup"><span data-stu-id="300a9-138">The name of the **printTaskDefinition**.</span></span>|
|<span data-ttu-id="300a9-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="300a9-139">createdBy</span></span>|<span data-ttu-id="300a9-140">String</span><span class="sxs-lookup"><span data-stu-id="300a9-140">String</span></span>|<span data-ttu-id="300a9-141">Сведения о приложении, создав определение задачи.</span><span class="sxs-lookup"><span data-stu-id="300a9-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="300a9-142">Только `createdBy.displayName` свойство может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="300a9-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="300a9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="300a9-143">Response</span></span>

<span data-ttu-id="300a9-144">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="300a9-144">If successful, this method returns a `200 OK` response code and an updated [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="300a9-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="300a9-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="300a9-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="300a9-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printtaskdefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
Content-Type: application/json
Content-length: 163

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```

### <a name="response"></a><span data-ttu-id="300a9-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="300a9-147">Response</span></span>
<span data-ttu-id="300a9-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="300a9-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId" : "479688a0-cc3a-4993-ab24-54c7c80b047e",
    "displayName": "Requesting App Display Name"
  }
}
```

