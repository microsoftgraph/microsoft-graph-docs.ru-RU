---
title: Список NamedItemCollection
description: Получение списка объектов nameditem.
ms.openlocfilehash: c4dbf671a1e4d6baedaffc35623f040d68ea3e32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026320"
---
# <a name="list-nameditemcollection"></a><span data-ttu-id="1d817-103">Список NamedItemCollection</span><span class="sxs-lookup"><span data-stu-id="1d817-103">List NamedItemCollection</span></span>

<span data-ttu-id="1d817-104">Получение списка объектов nameditem.</span><span class="sxs-lookup"><span data-stu-id="1d817-104">Retrieve a list of nameditem objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1d817-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d817-105">Permissions</span></span>
<span data-ttu-id="1d817-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d817-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d817-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d817-108">Permission type</span></span>      | <span data-ttu-id="1d817-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d817-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d817-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d817-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1d817-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d817-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1d817-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d817-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d817-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d817-113">Not supported.</span></span>    |
|<span data-ttu-id="1d817-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d817-114">Application</span></span> | <span data-ttu-id="1d817-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d817-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d817-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d817-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d817-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d817-117">Optional query parameters</span></span>
<span data-ttu-id="1d817-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1d817-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d817-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d817-119">Request headers</span></span>
| <span data-ttu-id="1d817-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1d817-120">Name</span></span>      |<span data-ttu-id="1d817-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1d817-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d817-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d817-122">Authorization</span></span>  | <span data-ttu-id="1d817-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d817-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d817-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1d817-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1d817-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1d817-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d817-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d817-128">Request body</span></span>
<span data-ttu-id="1d817-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d817-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d817-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d817-130">Response</span></span>

<span data-ttu-id="1d817-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [WorkbookNamedItem](../resources/nameditem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1d817-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d817-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1d817-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d817-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d817-133">Request</span></span>
<span data-ttu-id="1d817-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d817-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_nameditemcollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names
```
##### <a name="response"></a><span data-ttu-id="1d817-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d817-135">Response</span></span>
<span data-ttu-id="1d817-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1d817-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List NamedItemCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->