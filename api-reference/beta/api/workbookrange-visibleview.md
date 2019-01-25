---
title: 'workbookRange: visibleView'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b7ddea5635f8cf90e448d15223b5de51b0138f21
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525390"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="45feb-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="45feb-104">workbookRange: visibleView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="45feb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45feb-105">Permissions</span></span>
<span data-ttu-id="45feb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45feb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45feb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45feb-108">Permission type</span></span>      | <span data-ttu-id="45feb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45feb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45feb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45feb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="45feb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45feb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="45feb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45feb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45feb-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45feb-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="45feb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45feb-114">Application</span></span> | <span data-ttu-id="45feb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45feb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="45feb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45feb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="45feb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45feb-117">Request headers</span></span>
| <span data-ttu-id="45feb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="45feb-118">Name</span></span>       | <span data-ttu-id="45feb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="45feb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45feb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45feb-120">Authorization</span></span>  | <span data-ttu-id="45feb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45feb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45feb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="45feb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="45feb-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="45feb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45feb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45feb-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="45feb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="45feb-127">Response</span></span>

<span data-ttu-id="45feb-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [workbookRangeView](../resources/workbookrangeview.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="45feb-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45feb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="45feb-129">Example</span></span>
<span data-ttu-id="45feb-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="45feb-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="45feb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="45feb-131">Request</span></span>
<span data-ttu-id="45feb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45feb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="45feb-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="45feb-133">Response</span></span>
<span data-ttu-id="45feb-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="45feb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-visibleview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
