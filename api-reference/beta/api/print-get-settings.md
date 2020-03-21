---
title: Получение параметров
description: Получение параметров на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 675e0c41e0aa9605b0a6088e13be78e9d52d57be
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896377"
---
# <a name="get-settings"></a><span data-ttu-id="6c4f7-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="6c4f7-103">Get settings</span></span>

<span data-ttu-id="6c4f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c4f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c4f7-105">Получение параметров на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c4f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c4f7-106">Permissions</span></span>
<span data-ttu-id="6c4f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c4f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c4f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c4f7-109">Permission type</span></span> | <span data-ttu-id="6c4f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c4f7-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6c4f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c4f7-111">Delegated (work or school account)</span></span>| <span data-ttu-id="6c4f7-112">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6c4f7-112">Users.Read.All</span></span> |
|<span data-ttu-id="6c4f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c4f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c4f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-114">Not Supported.</span></span>|
|<span data-ttu-id="6c4f7-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6c4f7-115">Application</span></span>|<span data-ttu-id="6c4f7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c4f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c4f7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c4f7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c4f7-118">Optional query parameters</span></span>
<span data-ttu-id="6c4f7-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6c4f7-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6c4f7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c4f7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c4f7-121">Request headers</span></span>
| <span data-ttu-id="6c4f7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6c4f7-122">Name</span></span>      |<span data-ttu-id="6c4f7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6c4f7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c4f7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c4f7-124">Authorization</span></span> | <span data-ttu-id="6c4f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c4f7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c4f7-127">Request body</span></span>
<span data-ttu-id="6c4f7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6c4f7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c4f7-129">Response</span></span>
<span data-ttu-id="6c4f7-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтсеттингс](../resources/printsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-130">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c4f7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6c4f7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c4f7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c4f7-132">Request</span></span>
<span data-ttu-id="6c4f7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}-->
```http
GET https://graph.microsoft.com/beta/print/settings
```
##### <a name="response"></a><span data-ttu-id="6c4f7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c4f7-134">Response</span></span>
<span data-ttu-id="6c4f7-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-135">The following is an example of the response.</span></span>
><span data-ttu-id="6c4f7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c4f7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 144

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->