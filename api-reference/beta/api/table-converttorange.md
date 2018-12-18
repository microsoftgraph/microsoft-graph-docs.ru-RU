---
title: 'Table: convertToRange'
description: Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.
author: lumine2008
ms.openlocfilehash: 7f05f21427e75ef3e86981f0ca52d1364ec86bf0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306813"
---
# <a name="table-converttorange"></a><span data-ttu-id="6f3cb-104">Table: convertToRange</span><span class="sxs-lookup"><span data-stu-id="6f3cb-104">Table: convertToRange</span></span>

> <span data-ttu-id="6f3cb-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f3cb-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f3cb-p103">Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-p103">Converts the table into a normal range of cells. All data is preserved.</span></span>
## <a name="permissions"></a><span data-ttu-id="6f3cb-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f3cb-109">Permissions</span></span>
<span data-ttu-id="6f3cb-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f3cb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f3cb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f3cb-112">Permission type</span></span>      | <span data-ttu-id="6f3cb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f3cb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f3cb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f3cb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6f3cb-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f3cb-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6f3cb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f3cb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f3cb-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f3cb-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6f3cb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f3cb-118">Application</span></span> | <span data-ttu-id="6f3cb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f3cb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f3cb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/convertToRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/convertToRange

```
## <a name="request-headers"></a><span data-ttu-id="6f3cb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f3cb-121">Request headers</span></span>
| <span data-ttu-id="6f3cb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6f3cb-122">Name</span></span>       | <span data-ttu-id="6f3cb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6f3cb-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f3cb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f3cb-124">Authorization</span></span>  | <span data-ttu-id="6f3cb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6f3cb-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6f3cb-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="6f3cb-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f3cb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f3cb-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6f3cb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f3cb-131">Response</span></span>

<span data-ttu-id="6f3cb-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [Range](../resources/range.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-132">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f3cb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6f3cb-133">Example</span></span>
<span data-ttu-id="6f3cb-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6f3cb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f3cb-135">Request</span></span>
<span data-ttu-id="6f3cb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_converttorange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange
```

##### <a name="response"></a><span data-ttu-id="6f3cb-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f3cb-137">Response</span></span>
<span data-ttu-id="6f3cb-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6f3cb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Table: convertToRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->