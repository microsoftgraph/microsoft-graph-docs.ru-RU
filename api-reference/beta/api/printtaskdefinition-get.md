---
title: Получение Таскдефинитион
description: Получение сведений об определении задачи.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8105fa16971ed468e024291f97b529f2938df96c
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091660"
---
# <a name="get-taskdefinition"></a><span data-ttu-id="5d515-103">Получение Таскдефинитион</span><span class="sxs-lookup"><span data-stu-id="5d515-103">Get taskDefinition</span></span>

<span data-ttu-id="5d515-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d515-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d515-105">Получение сведений об определении задачи.</span><span class="sxs-lookup"><span data-stu-id="5d515-105">Get details about a task definition.</span></span>

<span data-ttu-id="5d515-106">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="5d515-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d515-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d515-107">Permissions</span></span>
<span data-ttu-id="5d515-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5d515-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5d515-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d515-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5d515-110">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="5d515-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="5d515-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d515-111">Permission type</span></span> | <span data-ttu-id="5d515-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d515-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5d515-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d515-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5d515-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d515-114">Not supported.</span></span> |
|<span data-ttu-id="5d515-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d515-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d515-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d515-116">Not Supported.</span></span>|
|<span data-ttu-id="5d515-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d515-117">Application</span></span>| <span data-ttu-id="5d515-118">Принттаскдефинитион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5d515-118">PrintTaskDefinition.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d515-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d515-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/taskDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5d515-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d515-120">Request headers</span></span>
| <span data-ttu-id="5d515-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5d515-121">Name</span></span>      |<span data-ttu-id="5d515-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5d515-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d515-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d515-123">Authorization</span></span> | <span data-ttu-id="5d515-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5d515-124">Bearer {token}.</span></span> <span data-ttu-id="5d515-125">Required.</span><span class="sxs-lookup"><span data-stu-id="5d515-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d515-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d515-126">Request body</span></span>
<span data-ttu-id="5d515-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d515-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5d515-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d515-128">Response</span></span>
<span data-ttu-id="5d515-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принттаскдефинитион](../resources/printtaskdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d515-129">If successful, this method returns a `200 OK` response code and a [printTaskDefinition](../resources/printtaskdefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d515-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5d515-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d515-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d515-131">Request</span></span>
<span data-ttu-id="5d515-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d515-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_taskdefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/taskDefinitions/fab143fd-ee61-4358-8558-2c7dee953982
```

---

### <a name="response"></a><span data-ttu-id="5d515-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d515-133">Response</span></span>
<span data-ttu-id="5d515-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d515-134">The following is an example of the response.</span></span>
><span data-ttu-id="5d515-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5d515-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5d515-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5d515-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 380

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/taskDefinitions/$entity",
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId": "815f204f-c791-4ee6-9098-614ecdb003f6",
    "displayName": "Requesting App Display Name"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
