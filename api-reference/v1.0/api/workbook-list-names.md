---
title: Список имен
description: Получение списка объектов nameditem.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 849df4780196f469ae54a6b26ee761d4cd5deffc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958896"
---
# <a name="list-names"></a><span data-ttu-id="ec69b-103">Список имен</span><span class="sxs-lookup"><span data-stu-id="ec69b-103">List names</span></span>

<span data-ttu-id="ec69b-104">Получение списка объектов nameditem.</span><span class="sxs-lookup"><span data-stu-id="ec69b-104">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec69b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec69b-105">Permissions</span></span>
<span data-ttu-id="ec69b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec69b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec69b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec69b-108">Permission type</span></span>      | <span data-ttu-id="ec69b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec69b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec69b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec69b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec69b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec69b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec69b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec69b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec69b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec69b-113">Not supported.</span></span>    |
|<span data-ttu-id="ec69b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec69b-114">Application</span></span> | <span data-ttu-id="ec69b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec69b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec69b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec69b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec69b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec69b-117">Optional query parameters</span></span>
<span data-ttu-id="ec69b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ec69b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec69b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec69b-119">Request headers</span></span>
| <span data-ttu-id="ec69b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ec69b-120">Name</span></span>      |<span data-ttu-id="ec69b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ec69b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec69b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec69b-122">Authorization</span></span>  | <span data-ttu-id="ec69b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec69b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec69b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec69b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec69b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="ec69b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec69b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec69b-128">Request body</span></span>
<span data-ttu-id="ec69b-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec69b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec69b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec69b-130">Response</span></span>

<span data-ttu-id="ec69b-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [WorkbookNamedItem](../resources/nameditem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ec69b-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec69b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ec69b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec69b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec69b-133">Request</span></span>
<span data-ttu-id="ec69b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec69b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names
```
##### <a name="response"></a><span data-ttu-id="ec69b-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ec69b-135">Response</span></span>
<span data-ttu-id="ec69b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ec69b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "value": [
    {
      "name": "name-value",
      "type": "type-value",
      "value": {
      },
      "visible": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
