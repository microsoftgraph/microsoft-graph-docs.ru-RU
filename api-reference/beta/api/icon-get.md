---
title: Получение объекта Icon
description: Получение свойств и связей объекта значка.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: d2d7d83fbadd9f86d261ddf918bc4d7bb59f4e33
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574036"
---
# <a name="get-icon"></a><span data-ttu-id="d7c94-103">Получение объекта Icon</span><span class="sxs-lookup"><span data-stu-id="d7c94-103">Get Icon</span></span>

<span data-ttu-id="d7c94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7c94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7c94-105">Получение свойств и связей объекта значка.</span><span class="sxs-lookup"><span data-stu-id="d7c94-105">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7c94-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7c94-106">Permissions</span></span>
<span data-ttu-id="d7c94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7c94-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7c94-109">Permission type</span></span>      | <span data-ttu-id="d7c94-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7c94-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7c94-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7c94-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d7c94-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7c94-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7c94-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7c94-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7c94-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7c94-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7c94-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7c94-115">Application</span></span> | <span data-ttu-id="d7c94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7c94-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7c94-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7c94-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7c94-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7c94-118">Optional query parameters</span></span>
<span data-ttu-id="d7c94-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d7c94-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7c94-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7c94-120">Request headers</span></span>
| <span data-ttu-id="d7c94-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d7c94-121">Name</span></span>      |<span data-ttu-id="d7c94-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d7c94-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7c94-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7c94-123">Authorization</span></span>  | <span data-ttu-id="d7c94-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7c94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7c94-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7c94-126">Request body</span></span>
<span data-ttu-id="d7c94-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7c94-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7c94-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7c94-128">Response</span></span>

<span data-ttu-id="d7c94-129">В случае успеха этот метод возвращает код отклика и `200 OK` [объект workbookIcon](../resources/workbookicon.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d7c94-129">If successful, this method returns a `200 OK` response code and [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7c94-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d7c94-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7c94-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7c94-131">Request</span></span>
<span data-ttu-id="d7c94-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7c94-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="d7c94-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7c94-133">Response</span></span>
<span data-ttu-id="d7c94-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7c94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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