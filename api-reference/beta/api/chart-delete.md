---
title: 'Chart: delete'
description: Удаляет объект диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3c2b0b051517e30e2a0275684124b26de0a355cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572124"
---
# <a name="chart-delete"></a><span data-ttu-id="67083-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="67083-103">Chart: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67083-104">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="67083-104">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="67083-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67083-105">Permissions</span></span>
<span data-ttu-id="67083-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67083-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67083-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67083-108">Permission type</span></span>      | <span data-ttu-id="67083-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67083-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67083-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67083-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67083-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67083-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67083-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67083-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67083-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67083-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67083-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67083-114">Application</span></span> | <span data-ttu-id="67083-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67083-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67083-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67083-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="67083-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67083-117">Request headers</span></span>
| <span data-ttu-id="67083-118">Имя</span><span class="sxs-lookup"><span data-stu-id="67083-118">Name</span></span>       | <span data-ttu-id="67083-119">Описание</span><span class="sxs-lookup"><span data-stu-id="67083-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67083-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67083-120">Authorization</span></span>  | <span data-ttu-id="67083-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67083-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67083-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="67083-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="67083-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="67083-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67083-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67083-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="67083-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="67083-127">Response</span></span>

<span data-ttu-id="67083-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="67083-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67083-130">Пример</span><span class="sxs-lookup"><span data-stu-id="67083-130">Example</span></span>
<span data-ttu-id="67083-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="67083-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="67083-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="67083-132">Request</span></span>
<span data-ttu-id="67083-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67083-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/delete
```

##### <a name="response"></a><span data-ttu-id="67083-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="67083-134">Response</span></span>
<span data-ttu-id="67083-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67083-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
