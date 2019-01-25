---
title: Создание объекта RangeBorder
description: С помощью этого API можно создать объект RangeBorder.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c7abc218ee6743b0b59c2b40714137d723649749
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519817"
---
# <a name="create-rangeborder"></a><span data-ttu-id="926b2-103">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="926b2-103">Create RangeBorder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="926b2-104">С помощью этого API можно создать объект RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="926b2-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="926b2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="926b2-105">Permissions</span></span>
<span data-ttu-id="926b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="926b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="926b2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="926b2-108">Permission type</span></span>      | <span data-ttu-id="926b2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="926b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="926b2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="926b2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="926b2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="926b2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="926b2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="926b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="926b2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="926b2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="926b2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="926b2-114">Application</span></span> | <span data-ttu-id="926b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="926b2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="926b2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="926b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="926b2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="926b2-117">Request headers</span></span>
| <span data-ttu-id="926b2-118">Имя</span><span class="sxs-lookup"><span data-stu-id="926b2-118">Name</span></span>       | <span data-ttu-id="926b2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="926b2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="926b2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="926b2-120">Authorization</span></span>  | <span data-ttu-id="926b2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="926b2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="926b2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="926b2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="926b2-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="926b2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="926b2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="926b2-126">Request body</span></span>
<span data-ttu-id="926b2-127">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="926b2-127">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="926b2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="926b2-128">Response</span></span>

<span data-ttu-id="926b2-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [RangeBorder](../resources/rangeborder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="926b2-129">If successful, this method returns `201 Created` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="926b2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="926b2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="926b2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="926b2-131">Request</span></span>
<span data-ttu-id="926b2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="926b2-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="926b2-133">Предоставьте в тексте запроса описание объекта [RangeBorder](../resources/rangeborder.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="926b2-133">In the request body, supply a JSON representation of [RangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="926b2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="926b2-134">Response</span></span>
<span data-ttu-id="926b2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="926b2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangeformat-post-borders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
