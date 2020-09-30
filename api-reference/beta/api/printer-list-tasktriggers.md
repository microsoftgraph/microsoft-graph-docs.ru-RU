---
title: Перечисление taskTriggers
description: Получение списка триггеров задач, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9a75e34d3134fab8e66c0c27d0e563d0a0d6750d
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314208"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="27f88-103">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="27f88-103">List taskTriggers</span></span>

<span data-ttu-id="27f88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27f88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27f88-105">Получение списка [триггеров задач](../resources/printtasktrigger.md) , связанных с [принтером](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="27f88-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="27f88-106">Список триггеров задач определяет, какие задачи будут вызываться в результате событий, происходящих во время печати.</span><span class="sxs-lookup"><span data-stu-id="27f88-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="27f88-107">Сведения о том, как использовать этот API для добавления поддержки печати по запросу к универсальной печати, [можно узнать в статье расширение универсальной печати для поддержки печати по запросу](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="27f88-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="27f88-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27f88-108">Permissions</span></span>
<span data-ttu-id="27f88-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27f88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="27f88-111">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="27f88-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="27f88-112">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="27f88-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="27f88-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27f88-113">Permission type</span></span> | <span data-ttu-id="27f88-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27f88-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="27f88-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27f88-115">Delegated (work or school account)</span></span>| <span data-ttu-id="27f88-116">Printer. Read. ALL, Printer. ReadWrite. ALL, Printer. FullControl. ALL.</span><span class="sxs-lookup"><span data-stu-id="27f88-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="27f88-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27f88-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27f88-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27f88-118">Not Supported.</span></span>|
|<span data-ttu-id="27f88-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27f88-119">Application</span></span>| <span data-ttu-id="27f88-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27f88-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27f88-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27f88-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27f88-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="27f88-122">Optional query parameters</span></span>
<span data-ttu-id="27f88-123">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="27f88-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="27f88-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="27f88-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="27f88-125">Exceptions</span><span class="sxs-lookup"><span data-stu-id="27f88-125">Exceptions</span></span>
<span data-ttu-id="27f88-126">Некоторые операторы не поддерживаются: `$count` , `$format` , `$search` , `$select` , `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="27f88-126">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27f88-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27f88-127">Request headers</span></span>
| <span data-ttu-id="27f88-128">Имя</span><span class="sxs-lookup"><span data-stu-id="27f88-128">Name</span></span>      |<span data-ttu-id="27f88-129">Описание</span><span class="sxs-lookup"><span data-stu-id="27f88-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27f88-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27f88-130">Authorization</span></span> | <span data-ttu-id="27f88-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27f88-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27f88-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27f88-133">Request body</span></span>
<span data-ttu-id="27f88-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27f88-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="27f88-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="27f88-135">Response</span></span>
<span data-ttu-id="27f88-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [принттасктригжер](../resources/printtasktrigger.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27f88-136">If successful, this method returns a `200 OK` response code and collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27f88-137">Пример</span><span class="sxs-lookup"><span data-stu-id="27f88-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="27f88-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="27f88-138">Request</span></span>
<span data-ttu-id="27f88-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27f88-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="27f88-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="27f88-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```
# <a name="c"></a>[<span data-ttu-id="27f88-141">C#</span><span class="sxs-lookup"><span data-stu-id="27f88-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktriggers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27f88-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27f88-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktriggers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27f88-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27f88-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktriggers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="27f88-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="27f88-144">Response</span></span>
<span data-ttu-id="27f88-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27f88-145">The following is an example of the response.</span></span>
><span data-ttu-id="27f88-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27f88-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('fcc7fe6a-5ba7-4059-8017-702f3a41c8a4')/taskTriggers",
  "value": [
    {
      "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
      "event": "jobStarted"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskTriggers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->