---
title: Создание объекта Chart
description: С помощью этого API можно создать объект Chart.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 27bd441e6002d69cf94f79b8e3de40f9614ad6a6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644065"
---
# <a name="create-chart"></a><span data-ttu-id="a7f61-103">Создание объекта Chart</span><span class="sxs-lookup"><span data-stu-id="a7f61-103">Create Chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7f61-104">С помощью этого API можно создать объект Chart.</span><span class="sxs-lookup"><span data-stu-id="a7f61-104">Use this API to create a new Chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7f61-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7f61-105">Permissions</span></span>
<span data-ttu-id="a7f61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7f61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7f61-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7f61-108">Permission type</span></span>      | <span data-ttu-id="a7f61-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7f61-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7f61-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7f61-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7f61-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7f61-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7f61-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7f61-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7f61-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7f61-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a7f61-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7f61-114">Application</span></span> | <span data-ttu-id="a7f61-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7f61-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7f61-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7f61-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/

```
## <a name="request-headers"></a><span data-ttu-id="a7f61-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7f61-117">Request headers</span></span>
| <span data-ttu-id="a7f61-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a7f61-118">Name</span></span>       | <span data-ttu-id="a7f61-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a7f61-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7f61-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7f61-120">Authorization</span></span>  | <span data-ttu-id="a7f61-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7f61-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7f61-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a7f61-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="a7f61-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a7f61-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7f61-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7f61-126">Request body</span></span>
<span data-ttu-id="a7f61-127">Предоставьте в тексте запроса описание объекта [Chart](../resources/chart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7f61-127">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a7f61-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7f61-128">Response</span></span>

<span data-ttu-id="a7f61-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Chart](../resources/chart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7f61-129">If successful, this method returns `201 Created` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7f61-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a7f61-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7f61-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7f61-131">Request</span></span>
<span data-ttu-id="a7f61-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7f61-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="a7f61-133">Предоставьте в тексте запроса описание объекта [Chart](../resources/chart.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7f61-133">In the request body, supply a JSON representation of [Chart](../resources/chart.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a7f61-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7f61-134">Response</span></span>
<span data-ttu-id="a7f61-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7f61-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-post-charts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
