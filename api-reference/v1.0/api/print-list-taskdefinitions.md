---
title: Перечисление taskDefinitions
description: Извлечение списка определений задач, определенных приложением-запросом в клиенте.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: b294d020c2200e080334e23e143c13943dabd62b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517517"
---
# <a name="list-taskdefinitions"></a><span data-ttu-id="d93ca-103">Перечисление taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="d93ca-103">List taskDefinitions</span></span>
<span data-ttu-id="d93ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d93ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d93ca-105">Извлечение списка [определений задач,](../resources/printtaskdefinition.md) определенных приложением-запросом в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d93ca-105">Retrieve a list of [task definitions](../resources/printtaskdefinition.md) that the requesting app defined in the tenant.</span></span>

<span data-ttu-id="d93ca-106">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="d93ca-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="d93ca-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d93ca-107">Permissions</span></span>
<span data-ttu-id="d93ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d93ca-110">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="d93ca-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d93ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d93ca-111">Permission type</span></span> | <span data-ttu-id="d93ca-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d93ca-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d93ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d93ca-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d93ca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d93ca-114">Not supported.</span></span> |
|<span data-ttu-id="d93ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d93ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d93ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d93ca-116">Not Supported.</span></span>|
|<span data-ttu-id="d93ca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d93ca-117">Application</span></span>| <span data-ttu-id="d93ca-118">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d93ca-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d93ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d93ca-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/taskDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d93ca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d93ca-120">Optional query parameters</span></span>
<span data-ttu-id="d93ca-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d93ca-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d93ca-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d93ca-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="d93ca-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="d93ca-123">Exceptions</span></span>
<span data-ttu-id="d93ca-124">Некоторые операторы не поддерживаются: `$count` , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="d93ca-124">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d93ca-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d93ca-125">Request headers</span></span>
|<span data-ttu-id="d93ca-126">Имя</span><span class="sxs-lookup"><span data-stu-id="d93ca-126">Name</span></span>|<span data-ttu-id="d93ca-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d93ca-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d93ca-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d93ca-128">Authorization</span></span>|<span data-ttu-id="d93ca-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d93ca-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d93ca-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d93ca-131">Request body</span></span>
<span data-ttu-id="d93ca-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d93ca-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d93ca-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d93ca-133">Response</span></span>

<span data-ttu-id="d93ca-134">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [printTaskDefinition](../resources/printtaskdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d93ca-134">If successful, this method returns a `200 OK` response code and a collection of [printTaskDefinition](../resources/printtaskdefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d93ca-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="d93ca-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d93ca-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d93ca-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printtaskdefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/taskDefinitions
```


### <a name="response"></a><span data-ttu-id="d93ca-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d93ca-137">Response</span></span>
<span data-ttu-id="d93ca-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d93ca-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printTaskDefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions",
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

