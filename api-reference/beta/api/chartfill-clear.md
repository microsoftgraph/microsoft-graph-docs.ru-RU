---
title: 'ChartFill: clear'
description: Очищает цвет заливки элемента диаграммы.
ms.openlocfilehash: afb83221969d3dcf6dc56212181c5807b22938ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075002"
---
# <a name="chartfill-clear"></a><span data-ttu-id="e5f62-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="e5f62-103">ChartFill: clear</span></span>

> <span data-ttu-id="e5f62-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5f62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5f62-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5f62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5f62-106">Очищает цвет заливки элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e5f62-106">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5f62-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5f62-107">Permissions</span></span>
<span data-ttu-id="e5f62-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5f62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5f62-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5f62-110">Permission type</span></span>      | <span data-ttu-id="e5f62-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5f62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5f62-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5f62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e5f62-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5f62-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5f62-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5f62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5f62-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5f62-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5f62-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5f62-116">Application</span></span> | <span data-ttu-id="e5f62-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5f62-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5f62-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5f62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="e5f62-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5f62-119">Request headers</span></span>
| <span data-ttu-id="e5f62-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e5f62-120">Name</span></span>       | <span data-ttu-id="e5f62-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e5f62-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5f62-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5f62-122">Authorization</span></span>  | <span data-ttu-id="e5f62-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5f62-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5f62-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5f62-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5f62-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e5f62-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5f62-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5f62-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e5f62-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5f62-129">Response</span></span>

<span data-ttu-id="e5f62-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e5f62-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5f62-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e5f62-132">Example</span></span>
<span data-ttu-id="e5f62-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e5f62-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5f62-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5f62-134">Request</span></span>
<span data-ttu-id="e5f62-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5f62-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="e5f62-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5f62-136">Response</span></span>
<span data-ttu-id="e5f62-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5f62-137">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->