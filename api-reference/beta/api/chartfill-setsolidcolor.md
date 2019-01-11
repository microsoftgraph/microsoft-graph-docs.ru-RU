---
title: 'ChartFill: setSolidColor'
description: Задает заливку одним цветом для элемента диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: ffd5d4f954fea72963c7d443a5df6de12f1dc516
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854644"
---
# <a name="chartfill-setsolidcolor"></a><span data-ttu-id="3c676-103">ChartFill: setSolidColor</span><span class="sxs-lookup"><span data-stu-id="3c676-103">ChartFill: setSolidColor</span></span>

> <span data-ttu-id="3c676-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c676-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c676-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c676-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c676-106">Задает заливку одним цветом для элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3c676-106">Sets the fill formatting of a chart element to a uniform color.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c676-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c676-107">Permissions</span></span>
<span data-ttu-id="3c676-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c676-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c676-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c676-110">Permission type</span></span>      | <span data-ttu-id="3c676-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c676-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c676-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c676-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c676-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c676-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3c676-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c676-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c676-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c676-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3c676-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c676-116">Application</span></span> | <span data-ttu-id="3c676-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c676-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c676-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c676-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/title/format/fill/setSolidColor
POST /workbook/worksheets/{id|name}/charts(<name>)/legend/format/fill/setSolidColor

```
## <a name="request-headers"></a><span data-ttu-id="3c676-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c676-119">Request headers</span></span>
| <span data-ttu-id="3c676-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3c676-120">Name</span></span>       | <span data-ttu-id="3c676-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3c676-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3c676-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c676-122">Authorization</span></span>  | <span data-ttu-id="3c676-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c676-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3c676-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3c676-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3c676-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="3c676-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c676-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c676-128">Request body</span></span>
<span data-ttu-id="3c676-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3c676-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c676-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="3c676-130">Parameter</span></span>    | <span data-ttu-id="3c676-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3c676-131">Type</span></span>   |<span data-ttu-id="3c676-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3c676-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c676-133">color</span><span class="sxs-lookup"><span data-stu-id="3c676-133">color</span></span>|<span data-ttu-id="3c676-134">строка</span><span class="sxs-lookup"><span data-stu-id="3c676-134">string</span></span>|<span data-ttu-id="3c676-135">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="3c676-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|

## <a name="response"></a><span data-ttu-id="3c676-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c676-136">Response</span></span>

<span data-ttu-id="3c676-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3c676-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c676-139">Пример</span><span class="sxs-lookup"><span data-stu-id="3c676-139">Example</span></span>
<span data-ttu-id="3c676-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="3c676-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3c676-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c676-141">Request</span></span>
<span data-ttu-id="3c676-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c676-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_setsolidcolor"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/format/fill/setSolidColor
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```

##### <a name="response"></a><span data-ttu-id="3c676-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c676-143">Response</span></span>
<span data-ttu-id="3c676-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c676-144">Here is an example of the response.</span></span> 
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
  "description": "ChartFill: setSolidColor",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
