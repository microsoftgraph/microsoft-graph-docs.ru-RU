---
title: 'TableSort: reapply'
description: Повторно применяет текущие параметры сортировки к таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: db2407d664f75fb06217170d86138bd52e745f2b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511333"
---
# <a name="tablesort-reapply"></a><span data-ttu-id="12fa9-103">TableSort: reapply</span><span class="sxs-lookup"><span data-stu-id="12fa9-103">TableSort: reapply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12fa9-104">Повторно применяет текущие параметры сортировки к таблице.</span><span class="sxs-lookup"><span data-stu-id="12fa9-104">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="12fa9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12fa9-105">Permissions</span></span>
<span data-ttu-id="12fa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fa9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12fa9-108">Permission type</span></span>      | <span data-ttu-id="12fa9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12fa9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12fa9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12fa9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="12fa9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12fa9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12fa9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12fa9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12fa9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12fa9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="12fa9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12fa9-114">Application</span></span> | <span data-ttu-id="12fa9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fa9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12fa9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12fa9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="12fa9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12fa9-117">Request headers</span></span>
| <span data-ttu-id="12fa9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="12fa9-118">Name</span></span>       | <span data-ttu-id="12fa9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="12fa9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12fa9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12fa9-120">Authorization</span></span>  | <span data-ttu-id="12fa9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12fa9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12fa9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="12fa9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="12fa9-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="12fa9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fa9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12fa9-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="12fa9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fa9-127">Response</span></span>

<span data-ttu-id="12fa9-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="12fa9-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12fa9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="12fa9-130">Example</span></span>
<span data-ttu-id="12fa9-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="12fa9-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="12fa9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="12fa9-132">Request</span></span>
<span data-ttu-id="12fa9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12fa9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```

##### <a name="response"></a><span data-ttu-id="12fa9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="12fa9-134">Response</span></span>
<span data-ttu-id="12fa9-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12fa9-135">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablesort-reapply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
