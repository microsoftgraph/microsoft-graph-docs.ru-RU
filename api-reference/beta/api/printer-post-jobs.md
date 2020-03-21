---
title: Создание printJob
description: Создание нового метода printJob для принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e1cae1610877ae9354729d31c0999185612c3b86
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896239"
---
# <a name="create-printjob"></a><span data-ttu-id="f54c2-103">Создание printJob</span><span class="sxs-lookup"><span data-stu-id="f54c2-103">Create printJob</span></span>

<span data-ttu-id="f54c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f54c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f54c2-105">Создание нового [метода printJob](../resources/printJob.md) для [принтера](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="f54c2-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="f54c2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f54c2-106">Permissions</span></span>
<span data-ttu-id="f54c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f54c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f54c2-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="f54c2-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="f54c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f54c2-110">Permission type</span></span> | <span data-ttu-id="f54c2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f54c2-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f54c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f54c2-112">Delegated (work or school account)</span></span>| <span data-ttu-id="f54c2-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f54c2-113">Users.Read.All</span></span> |
|<span data-ttu-id="f54c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f54c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f54c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f54c2-115">Not Supported.</span></span>|
|<span data-ttu-id="f54c2-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f54c2-116">Application</span></span>|<span data-ttu-id="f54c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f54c2-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f54c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f54c2-118">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="f54c2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f54c2-119">Request headers</span></span>
| <span data-ttu-id="f54c2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f54c2-120">Name</span></span>      |<span data-ttu-id="f54c2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f54c2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f54c2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f54c2-122">Authorization</span></span> | <span data-ttu-id="f54c2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f54c2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f54c2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f54c2-125">Content-type</span></span>  | <span data-ttu-id="f54c2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f54c2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f54c2-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="f54c2-128">Request body</span></span>
<span data-ttu-id="f54c2-129">В тексте запроса добавьте представление объекта [printJob](../resources/printjob.md) в формате JSON, включая один объект [printDocument](../resources/printDocument.md) .</span><span class="sxs-lookup"><span data-stu-id="f54c2-129">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object, including one [printDocument](../resources/printDocument.md) object.</span></span> <span data-ttu-id="f54c2-130">Задания и идентификаторы документов устанавливаются автоматически во время создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="f54c2-130">The job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="f54c2-131">Теперь для универсальной печати поддерживается только один **printDocument** для каждого объекта **printJob** .</span><span class="sxs-lookup"><span data-stu-id="f54c2-131">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="f54c2-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f54c2-132">Response</span></span>
<span data-ttu-id="f54c2-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [printJob](../resources/printjob.md) и связанный с [printDocument](../resources/printDocument.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f54c2-133">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="f54c2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f54c2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f54c2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f54c2-135">Request</span></span>
<span data-ttu-id="f54c2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f54c2-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
##### <a name="response"></a><span data-ttu-id="f54c2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f54c2-137">Response</span></span>
<span data-ttu-id="f54c2-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f54c2-138">The following is an example of the response.</span></span>
><span data-ttu-id="f54c2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f54c2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
