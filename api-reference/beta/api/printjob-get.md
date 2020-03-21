---
title: Получение printJob
description: Получение свойств и связей задания печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 011ba76e161d01ab3d168840163e8cb4f7a3a240
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896191"
---
# <a name="get-printjob"></a><span data-ttu-id="21b90-103">Получение printJob</span><span class="sxs-lookup"><span data-stu-id="21b90-103">Get printJob</span></span>

<span data-ttu-id="21b90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21b90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21b90-105">Получение свойств и связей задания печати.</span><span class="sxs-lookup"><span data-stu-id="21b90-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="21b90-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21b90-106">Permissions</span></span>
<span data-ttu-id="21b90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21b90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="21b90-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="21b90-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="21b90-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21b90-110">Permission type</span></span> | <span data-ttu-id="21b90-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21b90-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="21b90-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21b90-112">Delegated (work or school account)</span></span>| <span data-ttu-id="21b90-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="21b90-113">Users.Read.All</span></span> |
|<span data-ttu-id="21b90-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21b90-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21b90-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b90-115">Not Supported.</span></span>|
|<span data-ttu-id="21b90-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="21b90-116">Application</span></span>|<span data-ttu-id="21b90-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21b90-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21b90-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21b90-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="21b90-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21b90-119">Request headers</span></span>
| <span data-ttu-id="21b90-120">Имя</span><span class="sxs-lookup"><span data-stu-id="21b90-120">Name</span></span>      |<span data-ttu-id="21b90-121">Описание</span><span class="sxs-lookup"><span data-stu-id="21b90-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21b90-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21b90-122">Authorization</span></span> | <span data-ttu-id="21b90-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21b90-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21b90-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21b90-125">Request body</span></span>
<span data-ttu-id="21b90-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21b90-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="21b90-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="21b90-127">Response</span></span>
<span data-ttu-id="21b90-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [printJob](../resources/printjob.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21b90-128">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21b90-129">Пример</span><span class="sxs-lookup"><span data-stu-id="21b90-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21b90-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="21b90-130">Request</span></span>
<span data-ttu-id="21b90-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21b90-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}
```
##### <a name="response"></a><span data-ttu-id="21b90-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="21b90-132">Response</span></span>
<span data-ttu-id="21b90-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21b90-133">The following is an example of the response.</span></span>
><span data-ttu-id="21b90-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21b90-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 408

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {},
  "status": {
    "processingState": "completed",
    "processingStateDescription": "The print job has completed successfully and no further processing will take place."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->