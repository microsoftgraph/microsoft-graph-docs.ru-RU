---
title: Создание объекта ChartSeries
description: С помощью этого API можно создать объект ChartSeries.
author: lumine2008
ms.openlocfilehash: abf5f6a62d80592c3268996fb7d040c31172ae32
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346195"
---
# <a name="create-chartseries"></a><span data-ttu-id="928ed-103">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="928ed-103">Create ChartSeries</span></span>

> <span data-ttu-id="928ed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="928ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="928ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="928ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="928ed-106">С помощью этого API можно создать объект ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="928ed-106">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="928ed-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="928ed-107">Permissions</span></span>
<span data-ttu-id="928ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="928ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="928ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="928ed-110">Permission type</span></span>      | <span data-ttu-id="928ed-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="928ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="928ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="928ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="928ed-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="928ed-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="928ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="928ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="928ed-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="928ed-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="928ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="928ed-116">Application</span></span> | <span data-ttu-id="928ed-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="928ed-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="928ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="928ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series

```
## <a name="request-headers"></a><span data-ttu-id="928ed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="928ed-119">Request headers</span></span>
| <span data-ttu-id="928ed-120">Имя</span><span class="sxs-lookup"><span data-stu-id="928ed-120">Name</span></span>       | <span data-ttu-id="928ed-121">Описание</span><span class="sxs-lookup"><span data-stu-id="928ed-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="928ed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="928ed-122">Authorization</span></span>  | <span data-ttu-id="928ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="928ed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="928ed-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="928ed-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="928ed-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="928ed-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="928ed-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="928ed-128">Request body</span></span>
<span data-ttu-id="928ed-129">Предоставьте в тексте запроса описание объекта [ChartSeries](../resources/chartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="928ed-129">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="928ed-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="928ed-130">Response</span></span>

<span data-ttu-id="928ed-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ChartSeries](../resources/chartseries.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="928ed-131">If successful, this method returns `201 Created` response code and [ChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="928ed-132">Пример</span><span class="sxs-lookup"><span data-stu-id="928ed-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="928ed-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="928ed-133">Request</span></span>
<span data-ttu-id="928ed-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="928ed-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="928ed-135">Предоставьте в тексте запроса описание объекта [ChartSeries](../resources/chartseries.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="928ed-135">In the request body, supply a JSON representation of [ChartSeries](../resources/chartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="928ed-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="928ed-136">Response</span></span>
<span data-ttu-id="928ed-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="928ed-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->