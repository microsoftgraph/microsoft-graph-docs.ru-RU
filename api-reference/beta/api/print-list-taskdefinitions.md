---
title: Список Таскдефинитионс
description: Получение списка определений задач, которые запрашивает приложение, определенное в клиенте.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 91d00b7773b56d4c5f522981c7a59dde3744a710
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091726"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="0fd78-103">Список Таскдефинитионс</span><span class="sxs-lookup"><span data-stu-id="0fd78-103">List taskDefinitions</span></span>

<span data-ttu-id="0fd78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fd78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fd78-105">Получение списка [определений задач](../resources/printtaskdefinition.md) , которые запрашивает приложение, определенное в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0fd78-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="0fd78-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="0fd78-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="0fd78-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fd78-107">Permissions</span></span>
<span data-ttu-id="0fd78-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0fd78-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0fd78-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fd78-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0fd78-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="0fd78-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0fd78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fd78-111">Permission type</span></span> | <span data-ttu-id="0fd78-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fd78-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0fd78-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fd78-113">Delegated (work or school account)</span></span>| <span data-ttu-id="0fd78-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fd78-114">Not supported.</span></span> |
|<span data-ttu-id="0fd78-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fd78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fd78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fd78-116">Not Supported.</span></span>|
|<span data-ttu-id="0fd78-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fd78-117">Application</span></span>| <span data-ttu-id="0fd78-118">Принттаскдефинитион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0fd78-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fd78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fd78-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0fd78-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0fd78-120">Optional query parameters</span></span>
<span data-ttu-id="0fd78-121">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0fd78-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0fd78-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0fd78-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="0fd78-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="0fd78-123">Exceptions</span></span>
<span data-ttu-id="0fd78-124">Некоторые операторы не поддерживаются: `$count` , `$format` , `$search` , `$select` , `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="0fd78-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0fd78-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fd78-125">Request headers</span></span>
| <span data-ttu-id="0fd78-126">Имя</span><span class="sxs-lookup"><span data-stu-id="0fd78-126">Name</span></span>      |<span data-ttu-id="0fd78-127">Описание</span><span class="sxs-lookup"><span data-stu-id="0fd78-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0fd78-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fd78-128">Authorization</span></span> | <span data-ttu-id="0fd78-129">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0fd78-129">Bearer {token}.</span></span> <span data-ttu-id="0fd78-130">Required.</span><span class="sxs-lookup"><span data-stu-id="0fd78-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fd78-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fd78-131">Request body</span></span>
<span data-ttu-id="0fd78-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fd78-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0fd78-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fd78-133">Response</span></span>
<span data-ttu-id="0fd78-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принттаскдефинитион](../resources/printtaskdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fd78-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0fd78-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0fd78-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="0fd78-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fd78-136">Request</span></span>
<span data-ttu-id="0fd78-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fd78-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "print_list_taskdefinitions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions
```

---

### <a name="response"></a><span data-ttu-id="0fd78-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fd78-138">Response</span></span>
<span data-ttu-id="0fd78-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0fd78-139">The following is an example of the response.</span></span>
><span data-ttu-id="0fd78-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0fd78-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0fd78-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0fd78-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions",
  "value": [
    {
      "id": "fab143fd-ee61-4358-8558-2c7dee953982",
      "displayName": "Test TaskDefinitionName",
      "createdBy": {
        "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
        "displayName": "Requesting App Display Name"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
