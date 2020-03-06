---
title: 'Chart: delete'
description: Удаляет объект диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 68b514f41802f1c7b266cc9a3d13b5d2b34c81e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518590"
---
# <a name="chart-delete"></a><span data-ttu-id="dcf32-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="dcf32-103">Chart: delete</span></span>

<span data-ttu-id="dcf32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcf32-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dcf32-105">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="dcf32-105">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dcf32-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcf32-106">Permissions</span></span>
<span data-ttu-id="dcf32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcf32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcf32-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcf32-109">Permission type</span></span>      | <span data-ttu-id="dcf32-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcf32-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcf32-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcf32-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dcf32-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcf32-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dcf32-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcf32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcf32-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcf32-114">Not supported.</span></span>    |
|<span data-ttu-id="dcf32-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcf32-115">Application</span></span> | <span data-ttu-id="dcf32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcf32-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcf32-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcf32-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="dcf32-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcf32-118">Request headers</span></span>
| <span data-ttu-id="dcf32-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dcf32-119">Name</span></span>       | <span data-ttu-id="dcf32-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dcf32-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dcf32-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcf32-121">Authorization</span></span>  | <span data-ttu-id="dcf32-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcf32-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcf32-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dcf32-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dcf32-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dcf32-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcf32-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dcf32-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dcf32-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcf32-128">Response</span></span>

<span data-ttu-id="dcf32-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dcf32-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcf32-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dcf32-131">Example</span></span>
<span data-ttu-id="dcf32-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dcf32-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dcf32-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcf32-133">Request</span></span>
<span data-ttu-id="dcf32-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcf32-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/delete
```

##### <a name="response"></a><span data-ttu-id="dcf32-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcf32-135">Response</span></span>
<span data-ttu-id="dcf32-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcf32-136">Here is an example of the response.</span></span> 
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
