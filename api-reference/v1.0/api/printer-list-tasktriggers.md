---
title: Перечисление taskTriggers
description: Извлечение списка триггеров задач, связанных с принтером.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: b4f76f356120a27eb52dfd013b65cb7cd38ef43a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517391"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="0bc06-103">Перечисление taskTriggers</span><span class="sxs-lookup"><span data-stu-id="0bc06-103">List taskTriggers</span></span>
<span data-ttu-id="0bc06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bc06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0bc06-105">Извлечение списка [триггеров задач,](../resources/printtasktrigger.md) связанных с [принтером.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="0bc06-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="0bc06-106">Список триггеров задач определяет, какие задачи будут запускаться в результате событий, которые происходят во время печати.</span><span class="sxs-lookup"><span data-stu-id="0bc06-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="0bc06-107">Дополнительные сведения о том, как использовать этот API для добавления поддержки печати для тяги в Universal Print, см. в материале [Extending Universal Print to support pull printing.](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)</span><span class="sxs-lookup"><span data-stu-id="0bc06-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="0bc06-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0bc06-108">Permissions</span></span>
<span data-ttu-id="0bc06-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bc06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0bc06-111">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="0bc06-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="0bc06-112">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="0bc06-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0bc06-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bc06-113">Permission type</span></span> | <span data-ttu-id="0bc06-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bc06-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0bc06-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bc06-115">Delegated (work or school account)</span></span>| <span data-ttu-id="0bc06-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0bc06-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="0bc06-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bc06-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bc06-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bc06-118">Not Supported.</span></span>|
|<span data-ttu-id="0bc06-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bc06-119">Application</span></span>| <span data-ttu-id="0bc06-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bc06-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bc06-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bc06-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0bc06-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0bc06-122">Optional query parameters</span></span>
<span data-ttu-id="0bc06-123">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0bc06-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0bc06-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0bc06-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="0bc06-125">Exceptions</span><span class="sxs-lookup"><span data-stu-id="0bc06-125">Exceptions</span></span>
<span data-ttu-id="0bc06-126">Некоторые операторы не поддерживаются: `$count` , , , , `$format` `$search` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="0bc06-126">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0bc06-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bc06-127">Request headers</span></span>
|<span data-ttu-id="0bc06-128">Имя</span><span class="sxs-lookup"><span data-stu-id="0bc06-128">Name</span></span>|<span data-ttu-id="0bc06-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0bc06-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0bc06-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0bc06-130">Authorization</span></span>|<span data-ttu-id="0bc06-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bc06-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bc06-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0bc06-133">Request body</span></span>
<span data-ttu-id="0bc06-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0bc06-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bc06-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bc06-135">Response</span></span>

<span data-ttu-id="0bc06-136">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printTaskTrigger](../resources/printtasktrigger.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0bc06-136">If successful, this method returns a `200 OK` response code and a collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0bc06-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="0bc06-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0bc06-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bc06-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printtasktrigger"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers
```


### <a name="response"></a><span data-ttu-id="0bc06-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bc06-139">Response</span></span>
<span data-ttu-id="0bc06-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0bc06-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printTaskTrigger)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('fcc7fe6a-5ba7-4059-8017-702f3a41c8a4')/taskTriggers",
  "value": [
    {
      "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
      "event": "jobStarted"
    }
  ]
}
```

