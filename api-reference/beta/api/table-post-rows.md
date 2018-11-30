---
title: Создание объекта TableRow
description: 'Добавляет строки в конец таблицы. Обратите внимание на то, что API может принимать несколько строк данных, с помощью этот интерфейс API. Добавление одной строке за раз может привести к снижению производительности. Рекомендуемый подход бы для пакетной обработки строк в один вызов, а не выполнив одну строку вставки. Для достижения наилучших результатов собирать строки, чтобы вставить в части приложения и выполнить отдельных строк добавьте операции. Поэкспериментируйте с номером строки, чтобы определить, идеальная число строк для использования в одном вызове API. '
ms.openlocfilehash: c7a4340005f7eaea60d95c806475de92373e1364
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077035"
---
# <a name="create-tablerow"></a><span data-ttu-id="4b458-108">Создание объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="4b458-108">Create TableRow</span></span>

> <span data-ttu-id="4b458-109">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b458-109">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b458-110">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b458-110">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b458-111">Добавляет строки в конец таблицы.</span><span class="sxs-lookup"><span data-stu-id="4b458-111">Adds rows to the end of the table.</span></span> <span data-ttu-id="4b458-112">Обратите внимание на то, что API может принимать несколько строк данных, с помощью этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="4b458-112">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="4b458-113">Добавление одной строке за раз может привести к снижению производительности.</span><span class="sxs-lookup"><span data-stu-id="4b458-113">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="4b458-114">Рекомендуемый подход бы для пакетной обработки строк в один вызов, а не выполнив одну строку вставки.</span><span class="sxs-lookup"><span data-stu-id="4b458-114">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="4b458-115">Для достижения наилучших результатов собирать строки, чтобы вставить в части приложения и выполнить отдельных строк добавьте операции.</span><span class="sxs-lookup"><span data-stu-id="4b458-115">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="4b458-116">Поэкспериментируйте с номером строки, чтобы определить, идеальная число строк для использования в одном вызове API.</span><span class="sxs-lookup"><span data-stu-id="4b458-116">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="4b458-117">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="4b458-117">Error Handling</span></span>

<span data-ttu-id="4b458-118">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="4b458-118">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="4b458-119">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="4b458-119">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b458-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b458-120">Permissions</span></span>
<span data-ttu-id="4b458-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b458-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b458-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b458-123">Permission type</span></span>      | <span data-ttu-id="4b458-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b458-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b458-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b458-125">Delegated (work or school account)</span></span> | <span data-ttu-id="4b458-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b458-126">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b458-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b458-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b458-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b458-128">Not supported.</span></span>    |
|<span data-ttu-id="4b458-129">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b458-129">Application</span></span> | <span data-ttu-id="4b458-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b458-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b458-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b458-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="4b458-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b458-132">Request headers</span></span>
| <span data-ttu-id="4b458-133">Имя</span><span class="sxs-lookup"><span data-stu-id="4b458-133">Name</span></span>       | <span data-ttu-id="4b458-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4b458-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b458-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b458-135">Authorization</span></span>  | <span data-ttu-id="4b458-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b458-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4b458-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4b458-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="4b458-p107">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4b458-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b458-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b458-141">Request body</span></span>
<span data-ttu-id="4b458-142">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4b458-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4b458-143">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b458-143">Parameter</span></span>    | <span data-ttu-id="4b458-144">Тип</span><span class="sxs-lookup"><span data-stu-id="4b458-144">Type</span></span>   |<span data-ttu-id="4b458-145">Описание</span><span class="sxs-lookup"><span data-stu-id="4b458-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b458-146">index</span><span class="sxs-lookup"><span data-stu-id="4b458-146">index</span></span>|<span data-ttu-id="4b458-147">number</span><span class="sxs-lookup"><span data-stu-id="4b458-147">number</span></span>|<span data-ttu-id="4b458-p108">Необязательный параметр. Определяет относительную позицию новой строки. Если параметру присвоено значение null, строка добавляется в конце. Все строки ниже вставляемой строки сдвигаются вниз. Используется нулевой индекс.</span><span class="sxs-lookup"><span data-stu-id="4b458-p108">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="4b458-153">values</span><span class="sxs-lookup"><span data-stu-id="4b458-153">values</span></span>|<span data-ttu-id="4b458-154">(boolean, string или number)</span><span class="sxs-lookup"><span data-stu-id="4b458-154">(boolean or string or number)</span></span>|<span data-ttu-id="4b458-155">Двухмерный массив неформатированные значений строк таблицы.</span><span class="sxs-lookup"><span data-stu-id="4b458-155">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="4b458-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b458-156">Response</span></span>

<span data-ttu-id="4b458-157">В случае успеха этот метод возвращает код отклика `200 OK` и объект [TableRow](../resources/tablerow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b458-157">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b458-158">Пример</span><span class="sxs-lookup"><span data-stu-id="4b458-158">Example</span></span>
<span data-ttu-id="4b458-159">В этом примере в конец таблицы вставляются двух строк данных.</span><span class="sxs-lookup"><span data-stu-id="4b458-159">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="4b458-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b458-160">Request</span></span>
<span data-ttu-id="4b458-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b458-161">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4b458-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b458-162">Response</span></span>
<span data-ttu-id="4b458-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4b458-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
