---
title: Получение списка строк rangeView
description: Получение списка, который включает в себя объекты видимых ячеек в диапазоне.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c4c3b2f6a62427e3d30d9e157ba2deddcefa2a9c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937436"
---
# <a name="list-rangeview-rows"></a><span data-ttu-id="df37d-103">Получение списка строк rangeView</span><span class="sxs-lookup"><span data-stu-id="df37d-103">List rangeView rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df37d-104">Получение списка, который включает в себя объекты видимых ячеек в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="df37d-104">Retrieve a list of range view objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="df37d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df37d-105">Permissions</span></span>
<span data-ttu-id="df37d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df37d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df37d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df37d-108">Permission type</span></span>      | <span data-ttu-id="df37d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df37d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df37d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df37d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="df37d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df37d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df37d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df37d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df37d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df37d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="df37d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df37d-114">Application</span></span> | <span data-ttu-id="df37d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df37d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df37d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df37d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/rows

```
## <a name="optional-query-parameters"></a><span data-ttu-id="df37d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="df37d-117">Optional query parameters</span></span>
<span data-ttu-id="df37d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="df37d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df37d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df37d-119">Request headers</span></span>
| <span data-ttu-id="df37d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="df37d-120">Name</span></span>      |<span data-ttu-id="df37d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="df37d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df37d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df37d-122">Authorization</span></span>  | <span data-ttu-id="df37d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df37d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df37d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="df37d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="df37d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="df37d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df37d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df37d-128">Request body</span></span>
<span data-ttu-id="df37d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df37d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df37d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="df37d-130">Response</span></span>

<span data-ttu-id="df37d-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="df37d-131">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/workbookrangeview.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df37d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="df37d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df37d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="df37d-133">Request</span></span>
<span data-ttu-id="df37d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df37d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/rows 
```
##### <a name="response"></a><span data-ttu-id="df37d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="df37d-135">Response</span></span>
<span data-ttu-id="df37d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df37d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 247

{
  "value": [
    {
      "cellAddresses": "cellAddresses-value",
      "columnCount": 99,
      "formulas": "formulas-value",
      "formulasLocal": "formulasLocal-value",
      "formulasR1C1": "formulasR1C1-value",
      "index": 99
    }
  ]
}
```
