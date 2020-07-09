---
title: Обновление Таскдефинитион
description: Обновление определения задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c0f0140b23291b77a5c00ff42b209f1f2af89a67
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091720"
---
# <a name="update-taskdefinition"></a><span data-ttu-id="3e6c1-103">Обновление Таскдефинитион</span><span class="sxs-lookup"><span data-stu-id="3e6c1-103">Update taskDefinition</span></span>

<span data-ttu-id="3e6c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e6c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e6c1-105">Обновление определения задачи.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-105">Update a task definition.</span></span>

<span data-ttu-id="3e6c1-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="3e6c1-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="3e6c1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e6c1-107">Permissions</span></span>
<span data-ttu-id="3e6c1-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3e6c1-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e6c1-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3e6c1-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="3e6c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e6c1-111">Permission type</span></span> | <span data-ttu-id="3e6c1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e6c1-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3e6c1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e6c1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3e6c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-114">Not supported.</span></span> |
|<span data-ttu-id="3e6c1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e6c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e6c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-116">Not Supported.</span></span>|
|<span data-ttu-id="3e6c1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e6c1-117">Application</span></span>| <span data-ttu-id="3e6c1-118">Принттаскдефинитион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3e6c1-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e6c1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e6c1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3e6c1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e6c1-120">Request headers</span></span>
| <span data-ttu-id="3e6c1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3e6c1-121">Name</span></span>      |<span data-ttu-id="3e6c1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3e6c1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e6c1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e6c1-123">Authorization</span></span> | <span data-ttu-id="3e6c1-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-124">Bearer {token}.</span></span> <span data-ttu-id="3e6c1-125">Required.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-125">Required.</span></span> |
| <span data-ttu-id="3e6c1-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e6c1-126">Content-type</span></span>  | <span data-ttu-id="3e6c1-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-127">application/json.</span></span> <span data-ttu-id="3e6c1-128">Required.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e6c1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e6c1-129">Request body</span></span>
<span data-ttu-id="3e6c1-130">В тексте запроса укажите значения для соответствующих полей [принттаскдефинитион](../resources/printtaskdefinition.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-130">In the request body, supply the values for the relevant [printTaskDefinition](../resources/printtaskdefinition.md) fields that should be updated.</span></span> <span data-ttu-id="3e6c1-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3e6c1-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e6c1-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e6c1-133">Property</span></span>     | <span data-ttu-id="3e6c1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="3e6c1-134">Type</span></span>        | <span data-ttu-id="3e6c1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="3e6c1-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e6c1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3e6c1-136">displayName</span></span>|<span data-ttu-id="3e6c1-137">String</span><span class="sxs-lookup"><span data-stu-id="3e6c1-137">String</span></span>|<span data-ttu-id="3e6c1-138">Имя Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-138">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="3e6c1-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="3e6c1-139">createdBy</span></span>|<span data-ttu-id="3e6c1-140">String</span><span class="sxs-lookup"><span data-stu-id="3e6c1-140">String</span></span>|<span data-ttu-id="3e6c1-141">Сведения о приложении, которое создало определение задачи.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-141">Information about the app that created the task definition.</span></span> <span data-ttu-id="3e6c1-142">`createdBy.displayName`Можно обновить только свойство.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-142">Only the `createdBy.displayName` property can be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="3e6c1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e6c1-143">Response</span></span>
<span data-ttu-id="3e6c1-144">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-144">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="3e6c1-145">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-145">It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e6c1-146">Пример</span><span class="sxs-lookup"><span data-stu-id="3e6c1-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e6c1-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e6c1-147">Request</span></span>
<span data-ttu-id="3e6c1-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "print_update_taskdefinition"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
Content-type: application/json
Content-length: 122

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```

---

### <a name="response"></a><span data-ttu-id="3e6c1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e6c1-149">Response</span></span>
<span data-ttu-id="3e6c1-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3e6c1-150">The following is an example of the response.</span></span>
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
  "description": "Update taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
