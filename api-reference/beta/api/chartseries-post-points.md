---
title: Создание объекта ChartPoints
description: С помощью этого API можно создать объект ChartPoints.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 421df294710cda9ac07c4aea2f79c4d2c4ea9abc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575844"
---
# <a name="create-chartpoints"></a><span data-ttu-id="e71aa-103">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="e71aa-103">Create ChartPoints</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e71aa-104">С помощью этого API можно создать объект ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="e71aa-104">Use this API to create a new ChartPoints.</span></span>
## <a name="permissions"></a><span data-ttu-id="e71aa-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e71aa-105">Permissions</span></span>
<span data-ttu-id="e71aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e71aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e71aa-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e71aa-108">Permission type</span></span>      | <span data-ttu-id="e71aa-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e71aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e71aa-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e71aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e71aa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e71aa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e71aa-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e71aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e71aa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e71aa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e71aa-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e71aa-114">Application</span></span> | <span data-ttu-id="e71aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e71aa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e71aa-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e71aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points

```
## <a name="request-headers"></a><span data-ttu-id="e71aa-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e71aa-117">Request headers</span></span>
| <span data-ttu-id="e71aa-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e71aa-118">Name</span></span>       | <span data-ttu-id="e71aa-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e71aa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e71aa-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e71aa-120">Authorization</span></span>  | <span data-ttu-id="e71aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e71aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e71aa-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e71aa-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e71aa-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e71aa-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e71aa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e71aa-126">Request body</span></span>
<span data-ttu-id="e71aa-127">Предоставьте в тексте запроса описание объекта [ChartPoints](../resources/chartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e71aa-127">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e71aa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e71aa-128">Response</span></span>

<span data-ttu-id="e71aa-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [ChartPoints](../resources/chartpoint.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e71aa-129">If successful, this method returns `201 Created` response code and [ChartPoints](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e71aa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e71aa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e71aa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e71aa-131">Request</span></span>
<span data-ttu-id="e71aa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e71aa-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartpoints_from_chartseries"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/series(<undefined>)/points
Content-type: application/json
Content-length: 3

{
}
```
<span data-ttu-id="e71aa-133">Предоставьте в тексте запроса описание объекта [ChartPoints](../resources/chartpoint.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e71aa-133">In the request body, supply a JSON representation of [ChartPoints](../resources/chartpoint.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e71aa-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e71aa-134">Response</span></span>
<span data-ttu-id="e71aa-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e71aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartPoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartseries-post-points.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
