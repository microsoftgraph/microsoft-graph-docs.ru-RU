---
title: Получение Принтершаре
description: Получение свойств и связей общего ресурса принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c7799d4b712323cf2ad1b40ba2bd6ded7158dbfd
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896206"
---
# <a name="get-printershare"></a><span data-ttu-id="7c6d7-103">Получение Принтершаре</span><span class="sxs-lookup"><span data-stu-id="7c6d7-103">Get printerShare</span></span>

<span data-ttu-id="7c6d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c6d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c6d7-105">Получение свойств и связей общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c6d7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c6d7-106">Permissions</span></span>
<span data-ttu-id="7c6d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c6d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7c6d7-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="7c6d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c6d7-110">Permission type</span></span> | <span data-ttu-id="7c6d7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c6d7-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7c6d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c6d7-112">Delegated (work or school account)</span></span>| <span data-ttu-id="7c6d7-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="7c6d7-113">Users.Read.All</span></span> |
|<span data-ttu-id="7c6d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c6d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c6d7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-115">Not Supported.</span></span>|
|<span data-ttu-id="7c6d7-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7c6d7-116">Application</span></span>|<span data-ttu-id="7c6d7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c6d7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c6d7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printerShares/{id}
GET /print/printers/{id}/share
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c6d7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7c6d7-119">Optional query parameters</span></span>
<span data-ttu-id="7c6d7-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7c6d7-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7c6d7-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="7c6d7-122">Исключения</span><span class="sxs-lookup"><span data-stu-id="7c6d7-122">Exceptions</span></span>
* <span data-ttu-id="7c6d7-123">`$count` Оператор не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-123">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c6d7-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c6d7-124">Request headers</span></span>
| <span data-ttu-id="7c6d7-125">Имя</span><span class="sxs-lookup"><span data-stu-id="7c6d7-125">Name</span></span>      |<span data-ttu-id="7c6d7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7c6d7-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7c6d7-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c6d7-127">Authorization</span></span> | <span data-ttu-id="7c6d7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c6d7-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c6d7-130">Request body</span></span>
<span data-ttu-id="7c6d7-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7c6d7-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c6d7-132">Response</span></span>
<span data-ttu-id="7c6d7-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтершаре](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-133">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7c6d7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7c6d7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c6d7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c6d7-135">Request</span></span>
<span data-ttu-id="7c6d7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}-->
```http
GET https://graph.microsoft.com/beta/print/printerShares/{id}
```
##### <a name="response"></a><span data-ttu-id="7c6d7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c6d7-137">Response</span></span>
<span data-ttu-id="7c6d7-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-138">The following is an example of the response.</span></span>
><span data-ttu-id="7c6d7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c6d7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "name": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->