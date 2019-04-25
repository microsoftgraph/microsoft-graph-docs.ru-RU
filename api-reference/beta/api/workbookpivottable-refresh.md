---
title: 'workbookPivotTable: refresh'
description: Обновляет сводную таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4fc107f7b9b1679d89900a102e84e156443a38fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536140"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="c46bc-103">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="c46bc-103">workbookPivotTable: refresh</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c46bc-104">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="c46bc-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="c46bc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c46bc-105">Permissions</span></span>
<span data-ttu-id="c46bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c46bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c46bc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c46bc-108">Permission type</span></span>      | <span data-ttu-id="c46bc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c46bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c46bc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c46bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c46bc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c46bc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c46bc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c46bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c46bc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c46bc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c46bc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c46bc-114">Application</span></span> | <span data-ttu-id="c46bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c46bc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c46bc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c46bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="c46bc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c46bc-117">Request headers</span></span>
| <span data-ttu-id="c46bc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c46bc-118">Name</span></span>       | <span data-ttu-id="c46bc-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c46bc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c46bc-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c46bc-120">Authorization</span></span>  | <span data-ttu-id="c46bc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c46bc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c46bc-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c46bc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c46bc-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c46bc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c46bc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c46bc-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c46bc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c46bc-127">Response</span></span>

<span data-ttu-id="c46bc-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c46bc-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c46bc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c46bc-130">Example</span></span>
<span data-ttu-id="c46bc-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c46bc-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c46bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c46bc-132">Request</span></span>
<span data-ttu-id="c46bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c46bc-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="c46bc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c46bc-134">Response</span></span>
<span data-ttu-id="c46bc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c46bc-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookpivottable-refresh.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
