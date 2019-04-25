---
title: Создание объекта TableRow
description: 'Добавляет строки в конец таблицы. Обратите внимание, что API может принимать несколько строк данных с помощью этого API. Добавление по одной строке за раз может привести к ухудшению производительности. Рекомендуемый подход заключается в пакетировании строк в одном вызове, а не при вставке одиночной строки. Для достижения лучших результатов Соберите строки, которые необходимо вставить на стороне приложения, и выполните операцию добавления отдельных строк. ПоЭкспериментируйте с количеством строк, чтобы определить оптимальное количество строк для использования в едином вызове API. '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 88fd78516528f62925b18c1c45d9452404be6881
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536887"
---
# <a name="create-tablerow"></a><span data-ttu-id="807e7-108">Создание объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="807e7-108">Create TableRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="807e7-109">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="807e7-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="807e7-110">Обратите внимание, что API может принимать несколько строк данных с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="807e7-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="807e7-111">Добавление по одной строке за раз может привести к ухудшению производительности.</span><span class="sxs-lookup"><span data-stu-id="807e7-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="807e7-112">Рекомендуемый подход заключается в пакетировании строк в одном вызове, а не при вставке одиночной строки.</span><span class="sxs-lookup"><span data-stu-id="807e7-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="807e7-113">Для достижения лучших результатов Соберите строки, которые необходимо вставить на стороне приложения, и выполните операцию добавления отдельных строк.</span><span class="sxs-lookup"><span data-stu-id="807e7-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="807e7-114">ПоЭкспериментируйте с количеством строк, чтобы определить оптимальное количество строк для использования в едином вызове API.</span><span class="sxs-lookup"><span data-stu-id="807e7-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="807e7-115">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="807e7-115">Error Handling</span></span>

<span data-ttu-id="807e7-116">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="807e7-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="807e7-117">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="807e7-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="807e7-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="807e7-118">Permissions</span></span>
<span data-ttu-id="807e7-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="807e7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="807e7-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="807e7-121">Permission type</span></span>      | <span data-ttu-id="807e7-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="807e7-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="807e7-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="807e7-123">Delegated (work or school account)</span></span> | <span data-ttu-id="807e7-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="807e7-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="807e7-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="807e7-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="807e7-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="807e7-126">Not supported.</span></span>    |
|<span data-ttu-id="807e7-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="807e7-127">Application</span></span> | <span data-ttu-id="807e7-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="807e7-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="807e7-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="807e7-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="807e7-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="807e7-130">Request headers</span></span>
| <span data-ttu-id="807e7-131">Имя</span><span class="sxs-lookup"><span data-stu-id="807e7-131">Name</span></span>       | <span data-ttu-id="807e7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="807e7-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="807e7-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="807e7-133">Authorization</span></span>  | <span data-ttu-id="807e7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="807e7-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="807e7-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="807e7-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="807e7-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="807e7-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="807e7-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="807e7-139">Request body</span></span>
<span data-ttu-id="807e7-140">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="807e7-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="807e7-141">Параметр</span><span class="sxs-lookup"><span data-stu-id="807e7-141">Parameter</span></span>    | <span data-ttu-id="807e7-142">Тип</span><span class="sxs-lookup"><span data-stu-id="807e7-142">Type</span></span>   |<span data-ttu-id="807e7-143">Описание</span><span class="sxs-lookup"><span data-stu-id="807e7-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="807e7-144">index</span><span class="sxs-lookup"><span data-stu-id="807e7-144">index</span></span>|<span data-ttu-id="807e7-145">number</span><span class="sxs-lookup"><span data-stu-id="807e7-145">number</span></span>|<span data-ttu-id="807e7-p107">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="807e7-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="807e7-151">values</span><span class="sxs-lookup"><span data-stu-id="807e7-151">values</span></span>|<span data-ttu-id="807e7-152">(boolean, string или number)</span><span class="sxs-lookup"><span data-stu-id="807e7-152">(boolean or string or number)</span></span>|<span data-ttu-id="807e7-153">Двухмерный массив неформатированных значений строк таблицы.</span><span class="sxs-lookup"><span data-stu-id="807e7-153">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="807e7-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="807e7-154">Response</span></span>

<span data-ttu-id="807e7-155">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="807e7-155">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="807e7-156">Пример</span><span class="sxs-lookup"><span data-stu-id="807e7-156">Example</span></span>
<span data-ttu-id="807e7-157">В этом примере две строки данных вставляются в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="807e7-157">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="807e7-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="807e7-158">Request</span></span>
<span data-ttu-id="807e7-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="807e7-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="807e7-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="807e7-160">Response</span></span>
<span data-ttu-id="807e7-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="807e7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-post-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
