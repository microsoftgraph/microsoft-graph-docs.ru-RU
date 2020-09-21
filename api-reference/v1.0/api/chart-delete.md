---
title: 'Chart: delete'
description: Удаляет объект диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 72ffa27b7721ee17f6275dbed8f9a4ea60e196cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063837"
---
# <a name="chart-delete"></a><span data-ttu-id="a09c0-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="a09c0-103">Chart: delete</span></span>

<span data-ttu-id="a09c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a09c0-105">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a09c0-105">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a09c0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a09c0-106">Permissions</span></span>
<span data-ttu-id="a09c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a09c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09c0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a09c0-109">Permission type</span></span>      | <span data-ttu-id="a09c0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a09c0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a09c0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a09c0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a09c0-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a09c0-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a09c0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a09c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a09c0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a09c0-114">Not supported.</span></span>    |
|<span data-ttu-id="a09c0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a09c0-115">Application</span></span> | <span data-ttu-id="a09c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a09c0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a09c0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a09c0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="a09c0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a09c0-118">Request headers</span></span>
| <span data-ttu-id="a09c0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a09c0-119">Name</span></span>       | <span data-ttu-id="a09c0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a09c0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a09c0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a09c0-121">Authorization</span></span>  | <span data-ttu-id="a09c0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a09c0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a09c0-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a09c0-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a09c0-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a09c0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a09c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a09c0-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a09c0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a09c0-128">Response</span></span>

<span data-ttu-id="a09c0-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a09c0-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a09c0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a09c0-131">Example</span></span>
<span data-ttu-id="a09c0-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a09c0-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a09c0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a09c0-133">Request</span></span>
<span data-ttu-id="a09c0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a09c0-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/delete
```

##### <a name="response"></a><span data-ttu-id="a09c0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a09c0-135">Response</span></span>
<span data-ttu-id="a09c0-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a09c0-136">Here is an example of the response.</span></span> 
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

