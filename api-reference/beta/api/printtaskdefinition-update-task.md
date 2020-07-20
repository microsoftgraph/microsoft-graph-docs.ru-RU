---
title: Обновление задачи
description: Обновление задачи печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: cf25e219458d6b43583114041f8007d690be7685
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091663"
---
# <a name="update-task"></a><span data-ttu-id="6dd5f-103">Обновление задачи</span><span class="sxs-lookup"><span data-stu-id="6dd5f-103">Update task</span></span>

<span data-ttu-id="6dd5f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dd5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd5f-105">Обновление задачи печати.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-105">Update a print task.</span></span>

<span data-ttu-id="6dd5f-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="6dd5f-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="6dd5f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd5f-107">Permissions</span></span>
<span data-ttu-id="6dd5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6dd5f-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="6dd5f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd5f-111">Permission type</span></span> | <span data-ttu-id="6dd5f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dd5f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6dd5f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dd5f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="6dd5f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-114">Not supported.</span></span> |
|<span data-ttu-id="6dd5f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dd5f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dd5f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-116">Not Supported.</span></span>|
|<span data-ttu-id="6dd5f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dd5f-117">Application</span></span>| <span data-ttu-id="6dd5f-118">Принттаскдефинитион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6dd5f-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dd5f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dd5f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/taskDefinitions/{id}/tasks/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6dd5f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dd5f-120">Request headers</span></span>
| <span data-ttu-id="6dd5f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6dd5f-121">Name</span></span>      |<span data-ttu-id="6dd5f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd5f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6dd5f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dd5f-123">Authorization</span></span> | <span data-ttu-id="6dd5f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dd5f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6dd5f-126">Request body</span></span>
<span data-ttu-id="6dd5f-127">В тексте запроса укажите значения для соответствующих полей [принттаск](../resources/printtask.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-127">In the request body, supply the values for the relevant [printTask](../resources/printtask.md) fields that should be updated.</span></span> <span data-ttu-id="6dd5f-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6dd5f-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6dd5f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6dd5f-130">Property</span></span>     | <span data-ttu-id="6dd5f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6dd5f-131">Type</span></span>        | <span data-ttu-id="6dd5f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd5f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6dd5f-133">status</span><span class="sxs-lookup"><span data-stu-id="6dd5f-133">status</span></span>|<span data-ttu-id="6dd5f-134">String</span><span class="sxs-lookup"><span data-stu-id="6dd5f-134">String</span></span>|<span data-ttu-id="6dd5f-135">Include `state` и `description` Values, описывающие текущее состояние задачи.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-135">Include `state` and `description` values that describe the current state of the task.</span></span>|

## <a name="response"></a><span data-ttu-id="6dd5f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd5f-136">Response</span></span>
<span data-ttu-id="6dd5f-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6dd5f-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6dd5f-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="6dd5f-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dd5f-140">Request</span></span>
<span data-ttu-id="6dd5f-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_task"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3

{
  "status": {
    "state": "completed",
    "description": "completed"
  }
}
```

---

### <a name="response"></a><span data-ttu-id="6dd5f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd5f-142">Response</span></span>
<span data-ttu-id="6dd5f-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-143">The following is an example of the response.</span></span>
><span data-ttu-id="6dd5f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6dd5f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update task",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
