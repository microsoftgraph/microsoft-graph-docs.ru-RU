---
title: 'Chart: delete'
description: Удаляет объект диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2e7b7a6985eb653cf9ffec7ec1fd71dfb22e023e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578047"
---
# <a name="chart-delete"></a><span data-ttu-id="7e66b-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="7e66b-103">Chart: delete</span></span>

<span data-ttu-id="7e66b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e66b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e66b-105">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7e66b-105">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e66b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e66b-106">Permissions</span></span>
<span data-ttu-id="7e66b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e66b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e66b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e66b-109">Permission type</span></span>      | <span data-ttu-id="7e66b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e66b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e66b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e66b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e66b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e66b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e66b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e66b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e66b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e66b-114">Not supported.</span></span>    |
|<span data-ttu-id="7e66b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e66b-115">Application</span></span> | <span data-ttu-id="7e66b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e66b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e66b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e66b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}

```
## <a name="request-headers"></a><span data-ttu-id="7e66b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e66b-118">Request headers</span></span>
| <span data-ttu-id="7e66b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7e66b-119">Name</span></span>       | <span data-ttu-id="7e66b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7e66b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7e66b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e66b-121">Authorization</span></span>  | <span data-ttu-id="7e66b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e66b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e66b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7e66b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7e66b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7e66b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e66b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e66b-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7e66b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e66b-128">Response</span></span>

<span data-ttu-id="7e66b-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7e66b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e66b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7e66b-131">Example</span></span>
<span data-ttu-id="7e66b-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7e66b-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7e66b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e66b-133">Request</span></span>
<span data-ttu-id="7e66b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e66b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
```

##### <a name="response"></a><span data-ttu-id="7e66b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e66b-135">Response</span></span>
<span data-ttu-id="7e66b-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e66b-136">Here is an example of the response.</span></span> 
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
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

