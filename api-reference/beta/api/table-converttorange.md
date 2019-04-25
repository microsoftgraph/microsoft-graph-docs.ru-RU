---
title: 'Table: convertToRange'
description: Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2987f01767dffaeacc0e783049116765165e4630
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545382"
---
# <a name="table-converttorange"></a><span data-ttu-id="03664-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="03664-104">Table: convertToRange</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03664-p102">Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.</span><span class="sxs-lookup"><span data-stu-id="03664-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="03664-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03664-107">Permissions</span></span>
<span data-ttu-id="03664-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03664-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03664-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03664-110">Permission type</span></span>      | <span data-ttu-id="03664-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03664-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03664-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03664-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03664-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03664-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03664-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03664-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03664-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03664-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03664-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03664-116">Application</span></span> | <span data-ttu-id="03664-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03664-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03664-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03664-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="03664-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03664-119">Request headers</span></span>
| <span data-ttu-id="03664-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03664-120">Name</span></span>       | <span data-ttu-id="03664-121">Описание</span><span class="sxs-lookup"><span data-stu-id="03664-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03664-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03664-122">Authorization</span></span>  | <span data-ttu-id="03664-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03664-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03664-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="03664-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="03664-p105">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="03664-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03664-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03664-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="03664-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="03664-129">Response</span></span>

<span data-ttu-id="03664-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03664-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03664-131">Пример</span><span class="sxs-lookup"><span data-stu-id="03664-131">Example</span></span>
<span data-ttu-id="03664-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="03664-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03664-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="03664-133">Request</span></span>
<span data-ttu-id="03664-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03664-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="03664-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="03664-135">Response</span></span>
<span data-ttu-id="03664-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03664-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-converttorange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
