---
title: Получение объекта Icon
description: Получение свойств и связей объекта значка.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 8909f1fb610a664c4d2fe95f73a74abc4707f75c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953257"
---
# <a name="get-icon"></a><span data-ttu-id="2642e-103">Получение объекта Icon</span><span class="sxs-lookup"><span data-stu-id="2642e-103">Get Icon</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2642e-104">Получение свойств и связей объекта значка.</span><span class="sxs-lookup"><span data-stu-id="2642e-104">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2642e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2642e-105">Permissions</span></span>
<span data-ttu-id="2642e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2642e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2642e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2642e-108">Permission type</span></span>      | <span data-ttu-id="2642e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2642e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2642e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2642e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2642e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2642e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2642e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2642e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2642e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2642e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2642e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2642e-114">Application</span></span> | <span data-ttu-id="2642e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2642e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2642e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2642e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2642e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2642e-117">Optional query parameters</span></span>
<span data-ttu-id="2642e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2642e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2642e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2642e-119">Request headers</span></span>
| <span data-ttu-id="2642e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2642e-120">Name</span></span>      |<span data-ttu-id="2642e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2642e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2642e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2642e-122">Authorization</span></span>  | <span data-ttu-id="2642e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2642e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2642e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2642e-125">Request body</span></span>
<span data-ttu-id="2642e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2642e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2642e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="2642e-127">Response</span></span>

<span data-ttu-id="2642e-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [воркбукикон](../resources/workbookicon.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2642e-128">If successful, this method returns a `200 OK` response code and [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2642e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2642e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2642e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2642e-130">Request</span></span>
<span data-ttu-id="2642e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2642e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="2642e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2642e-132">Response</span></span>
<span data-ttu-id="2642e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2642e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
