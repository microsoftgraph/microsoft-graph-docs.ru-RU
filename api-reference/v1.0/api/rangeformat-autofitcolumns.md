---
title: 'RangeFormat: autofitColumns'
description: Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.
localization_priority: Normal
ms.openlocfilehash: e20f7cfc365b189ee4851c099cacd11158fc8ee6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881041"
---
# <a name="rangeformat-autofitcolumns"></a><span data-ttu-id="f1da4-103">RangeFormat: autofitColumns</span><span class="sxs-lookup"><span data-stu-id="f1da4-103">RangeFormat: autofitColumns</span></span>

<span data-ttu-id="f1da4-104">Изменяет ширину столбцов текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="f1da4-104">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1da4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1da4-105">Permissions</span></span>
<span data-ttu-id="f1da4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1da4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1da4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1da4-108">Permission type</span></span>      | <span data-ttu-id="f1da4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1da4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1da4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1da4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1da4-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1da4-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f1da4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1da4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1da4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1da4-113">Not supported.</span></span>    |
|<span data-ttu-id="f1da4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1da4-114">Application</span></span> | <span data-ttu-id="f1da4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1da4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1da4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1da4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/autofitColumns
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitColumns
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitColumns

```
## <a name="request-headers"></a><span data-ttu-id="f1da4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1da4-117">Request headers</span></span>
| <span data-ttu-id="f1da4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f1da4-118">Name</span></span>       | <span data-ttu-id="f1da4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f1da4-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f1da4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1da4-120">Authorization</span></span>  | <span data-ttu-id="f1da4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1da4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f1da4-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f1da4-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f1da4-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="f1da4-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1da4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1da4-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f1da4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1da4-127">Response</span></span>

<span data-ttu-id="f1da4-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f1da4-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1da4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f1da4-130">Example</span></span>
<span data-ttu-id="f1da4-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f1da4-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f1da4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1da4-132">Request</span></span>
<span data-ttu-id="f1da4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1da4-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitcolumns"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/autofitColumns
```

##### <a name="response"></a><span data-ttu-id="f1da4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1da4-134">Response</span></span>
<span data-ttu-id="f1da4-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f1da4-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitColumns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
