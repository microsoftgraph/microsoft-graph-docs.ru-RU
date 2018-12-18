---
title: Создание объекта Chart
description: С помощью этого API можно создать объект Chart.
author: lumine2008
ms.openlocfilehash: abc58613e87c6765a83db62178e54ef58ce425d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306771"
---
# <a name="create-chart"></a><span data-ttu-id="20b55-103">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="20b55-103">Create Chart</span></span>

> <span data-ttu-id="20b55-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20b55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20b55-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20b55-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20b55-106">С помощью этого API можно создать объект Chart.</span><span class="sxs-lookup"><span data-stu-id="20b55-106">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="20b55-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20b55-107">Permissions</span></span>
<span data-ttu-id="20b55-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20b55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20b55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20b55-110">Permission type</span></span>      | <span data-ttu-id="20b55-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20b55-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20b55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20b55-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20b55-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20b55-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20b55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20b55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20b55-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20b55-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20b55-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20b55-116">Application</span></span> | <span data-ttu-id="20b55-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20b55-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20b55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20b55-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="20b55-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20b55-119">Request headers</span></span>
| <span data-ttu-id="20b55-120">Имя</span><span class="sxs-lookup"><span data-stu-id="20b55-120">Name</span></span>       | <span data-ttu-id="20b55-121">Описание</span><span class="sxs-lookup"><span data-stu-id="20b55-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20b55-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20b55-122">Authorization</span></span>  | <span data-ttu-id="20b55-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20b55-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20b55-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20b55-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="20b55-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="20b55-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20b55-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20b55-128">Request body</span></span>
<span data-ttu-id="20b55-129">Предоставьте в тексте запроса описание объекта [Chart](../resources/chart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20b55-129">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="20b55-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="20b55-130">Response</span></span>

<span data-ttu-id="20b55-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20b55-131">If successful, this method returns `201 Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20b55-132">Пример</span><span class="sxs-lookup"><span data-stu-id="20b55-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20b55-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="20b55-133">Request</span></span>
<span data-ttu-id="20b55-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20b55-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chart_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```
<span data-ttu-id="20b55-135">Предоставьте в тексте запроса описание объекта [Chart](../resources/chart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20b55-135">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="20b55-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="20b55-136">Response</span></span>
<span data-ttu-id="20b55-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20b55-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->