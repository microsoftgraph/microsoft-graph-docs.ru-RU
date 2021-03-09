---
title: 'Chart: delete'
description: Удаляет объект диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a270319dcad87451c90258203eb13b4817908783
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574845"
---
# <a name="chart-delete"></a><span data-ttu-id="9f26a-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="9f26a-103">Chart: delete</span></span>

<span data-ttu-id="9f26a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f26a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f26a-105">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9f26a-105">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f26a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f26a-106">Permissions</span></span>
<span data-ttu-id="9f26a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f26a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f26a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f26a-109">Permission type</span></span>      | <span data-ttu-id="9f26a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f26a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f26a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f26a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f26a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f26a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f26a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f26a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f26a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f26a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9f26a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f26a-115">Application</span></span> | <span data-ttu-id="9f26a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f26a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f26a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f26a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
DELETE /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}
```
## <a name="request-headers"></a><span data-ttu-id="9f26a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f26a-118">Request headers</span></span>
| <span data-ttu-id="9f26a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f26a-119">Name</span></span>       | <span data-ttu-id="9f26a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9f26a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9f26a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f26a-121">Authorization</span></span>  | <span data-ttu-id="9f26a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f26a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f26a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9f26a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9f26a-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9f26a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f26a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f26a-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9f26a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f26a-128">Response</span></span>

<span data-ttu-id="9f26a-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9f26a-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f26a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9f26a-131">Example</span></span>
<span data-ttu-id="9f26a-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9f26a-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9f26a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f26a-133">Request</span></span>
<span data-ttu-id="9f26a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f26a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
```

##### <a name="response"></a><span data-ttu-id="9f26a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f26a-135">Response</span></span>
<span data-ttu-id="9f26a-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f26a-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


