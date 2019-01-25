---
title: 'TableSort: apply'
description: Выполняет сортировку.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2279109f83758958cb00940604854c4edeecd45
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523444"
---
# <a name="tablesort-apply"></a><span data-ttu-id="e13bd-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="e13bd-103">TableSort: apply</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e13bd-104">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="e13bd-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="e13bd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e13bd-105">Permissions</span></span>
<span data-ttu-id="e13bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e13bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e13bd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e13bd-108">Permission type</span></span>      | <span data-ttu-id="e13bd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e13bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e13bd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e13bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e13bd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e13bd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e13bd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e13bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e13bd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e13bd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e13bd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e13bd-114">Application</span></span> | <span data-ttu-id="e13bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e13bd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e13bd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e13bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="e13bd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e13bd-117">Request headers</span></span>
| <span data-ttu-id="e13bd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e13bd-118">Name</span></span>       | <span data-ttu-id="e13bd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e13bd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e13bd-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e13bd-120">Authorization</span></span>  | <span data-ttu-id="e13bd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e13bd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e13bd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e13bd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e13bd-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e13bd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e13bd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e13bd-126">Request body</span></span>
<span data-ttu-id="e13bd-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e13bd-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e13bd-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="e13bd-128">Parameter</span></span>    | <span data-ttu-id="e13bd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e13bd-129">Type</span></span>   |<span data-ttu-id="e13bd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e13bd-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e13bd-131">fields</span><span class="sxs-lookup"><span data-stu-id="e13bd-131">fields</span></span>|<span data-ttu-id="e13bd-132">SortField</span><span class="sxs-lookup"><span data-stu-id="e13bd-132">SortField</span></span>|<span data-ttu-id="e13bd-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="e13bd-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="e13bd-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="e13bd-134">matchCase</span></span>|<span data-ttu-id="e13bd-135">boolean</span><span class="sxs-lookup"><span data-stu-id="e13bd-135">boolean</span></span>|<span data-ttu-id="e13bd-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="e13bd-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="e13bd-138">method</span><span class="sxs-lookup"><span data-stu-id="e13bd-138">method</span></span>|<span data-ttu-id="e13bd-139">string</span><span class="sxs-lookup"><span data-stu-id="e13bd-139">string</span></span>|<span data-ttu-id="e13bd-p105">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="e13bd-p105">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="e13bd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e13bd-143">Response</span></span>

<span data-ttu-id="e13bd-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e13bd-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e13bd-146">Пример</span><span class="sxs-lookup"><span data-stu-id="e13bd-146">Example</span></span>
<span data-ttu-id="e13bd-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e13bd-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e13bd-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="e13bd-148">Request</span></span>
<span data-ttu-id="e13bd-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e13bd-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
Content-type: application/json
Content-length: 298

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="e13bd-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="e13bd-150">Response</span></span>
<span data-ttu-id="e13bd-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e13bd-151">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablesort-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
