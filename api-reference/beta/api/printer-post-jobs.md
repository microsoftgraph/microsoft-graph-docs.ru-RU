---
title: Создание printJob
description: Создание нового метода printJob для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: bf7ef738b82482caddef6a64e1c0f0f8eeb47c27
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947784"
---
# <a name="create-printjob"></a><span data-ttu-id="f44fe-103">Создание printJob</span><span class="sxs-lookup"><span data-stu-id="f44fe-103">Create printJob</span></span>

<span data-ttu-id="f44fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f44fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f44fe-105">Создание нового [метода printJob](../resources/printJob.md) для [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="f44fe-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="f44fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f44fe-106">Permissions</span></span>
<span data-ttu-id="f44fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f44fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f44fe-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="f44fe-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f44fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f44fe-110">Permission type</span></span> | <span data-ttu-id="f44fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f44fe-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f44fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f44fe-112">Delegated (work or school account)</span></span>| <span data-ttu-id="f44fe-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f44fe-113">Users.Read.All</span></span> |
|<span data-ttu-id="f44fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f44fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f44fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f44fe-115">Not Supported.</span></span>|
|<span data-ttu-id="f44fe-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f44fe-116">Application</span></span>|<span data-ttu-id="f44fe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f44fe-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f44fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f44fe-118">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="f44fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f44fe-119">Request headers</span></span>
| <span data-ttu-id="f44fe-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f44fe-120">Name</span></span>      |<span data-ttu-id="f44fe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f44fe-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f44fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f44fe-122">Authorization</span></span> | <span data-ttu-id="f44fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f44fe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f44fe-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f44fe-125">Content-type</span></span>  | <span data-ttu-id="f44fe-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f44fe-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f44fe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f44fe-128">Request body</span></span>
<span data-ttu-id="f44fe-129">В тексте запроса добавьте представление объекта [printJob](../resources/printjob.md) в формате JSON, включая один объект [printDocument](../resources/printDocument.md) .</span><span class="sxs-lookup"><span data-stu-id="f44fe-129">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object, including one [printDocument](../resources/printDocument.md) object.</span></span> <span data-ttu-id="f44fe-130">Задания и идентификаторы документов устанавливаются автоматически во время создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="f44fe-130">The job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="f44fe-131">Теперь для универсальной печати поддерживается только один **printDocument** для каждого объекта **printJob** .</span><span class="sxs-lookup"><span data-stu-id="f44fe-131">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="f44fe-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f44fe-132">Response</span></span>
<span data-ttu-id="f44fe-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [printJob](../resources/printjob.md) и связанный с [printDocument](../resources/printDocument.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f44fe-133">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="f44fe-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f44fe-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f44fe-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f44fe-135">Request</span></span>
<span data-ttu-id="f44fe-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f44fe-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f44fe-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f44fe-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="javascript"></a>[<span data-ttu-id="f44fe-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f44fe-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f44fe-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f44fe-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f44fe-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f44fe-140">Response</span></span>
<span data-ttu-id="f44fe-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f44fe-141">The following is an example of the response.</span></span>
><span data-ttu-id="f44fe-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f44fe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 425

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printJobs/$entity",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
      }
    }
  ]
}
```
