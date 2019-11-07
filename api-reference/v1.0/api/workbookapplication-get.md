---
title: Получение Воркбукаппликатион
description: Получение свойств и связей объекта Воркбукаппликатион.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f265fe51ce37504b331ee735f9d3fa91979f5891
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023236"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="72b8a-103">Получение Воркбукаппликатион</span><span class="sxs-lookup"><span data-stu-id="72b8a-103">Get workbookApplication</span></span>

<span data-ttu-id="72b8a-104">Получение свойств и связей объекта [воркбукаппликатион](../resources/workbookapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="72b8a-104">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="72b8a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72b8a-105">Permissions</span></span>
<span data-ttu-id="72b8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72b8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72b8a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72b8a-108">Permission type</span></span>      | <span data-ttu-id="72b8a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72b8a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72b8a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72b8a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72b8a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72b8a-111">Files.ReadWrite</span></span>   |
|<span data-ttu-id="72b8a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72b8a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72b8a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72b8a-113">Not supported.</span></span>    |
|<span data-ttu-id="72b8a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72b8a-114">Application</span></span> | <span data-ttu-id="72b8a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72b8a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72b8a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72b8a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="72b8a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72b8a-117">Request headers</span></span>
| <span data-ttu-id="72b8a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="72b8a-118">Name</span></span>      |<span data-ttu-id="72b8a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="72b8a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72b8a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72b8a-120">Authorization</span></span>  | <span data-ttu-id="72b8a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72b8a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72b8a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72b8a-123">Request body</span></span>
<span data-ttu-id="72b8a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72b8a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72b8a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="72b8a-125">Response</span></span>

<span data-ttu-id="72b8a-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукаппликатион](../resources/workbookapplication.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72b8a-126">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72b8a-127">Пример</span><span class="sxs-lookup"><span data-stu-id="72b8a-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="72b8a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="72b8a-128">Request</span></span>
<span data-ttu-id="72b8a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72b8a-129">Here is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```

### <a name="response"></a><span data-ttu-id="72b8a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="72b8a-130">Response</span></span>
<span data-ttu-id="72b8a-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72b8a-131">Here is an example of the response.</span></span> 

> <span data-ttu-id="72b8a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72b8a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
