---
title: 'TableCollection: add'
description: Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.
ms.openlocfilehash: 6435abe4a2671ec3937b7f1b0bbda8825fad1c7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081504"
---
# <a name="tablecollection-add"></a><span data-ttu-id="cebcb-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="cebcb-105">TableCollection: add</span></span>

> <span data-ttu-id="cebcb-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cebcb-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cebcb-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cebcb-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cebcb-p103">Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cebcb-p103">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="cebcb-111">Обработка ошибок</span><span class="sxs-lookup"><span data-stu-id="cebcb-111">Error Handling</span></span>

<span data-ttu-id="cebcb-112">Иногда при выполнении этого запроса может отображаться сообщение об ошибке 504 HTTP.</span><span class="sxs-lookup"><span data-stu-id="cebcb-112">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="cebcb-113">В этом случае нужно повторить запрос.</span><span class="sxs-lookup"><span data-stu-id="cebcb-113">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="cebcb-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cebcb-114">Permissions</span></span>
<span data-ttu-id="cebcb-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cebcb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cebcb-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cebcb-117">Permission type</span></span>      | <span data-ttu-id="cebcb-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cebcb-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cebcb-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cebcb-119">Delegated (work or school account)</span></span> | <span data-ttu-id="cebcb-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cebcb-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cebcb-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cebcb-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cebcb-122">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cebcb-122">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cebcb-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cebcb-123">Application</span></span> | <span data-ttu-id="cebcb-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cebcb-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cebcb-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cebcb-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="cebcb-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cebcb-126">Request headers</span></span>
| <span data-ttu-id="cebcb-127">Имя</span><span class="sxs-lookup"><span data-stu-id="cebcb-127">Name</span></span>       | <span data-ttu-id="cebcb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cebcb-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cebcb-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cebcb-129">Authorization</span></span>  | <span data-ttu-id="cebcb-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cebcb-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cebcb-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cebcb-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="cebcb-p107">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cebcb-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cebcb-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cebcb-135">Request body</span></span>
<span data-ttu-id="cebcb-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cebcb-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cebcb-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="cebcb-137">Parameter</span></span>    | <span data-ttu-id="cebcb-138">Тип</span><span class="sxs-lookup"><span data-stu-id="cebcb-138">Type</span></span>   |<span data-ttu-id="cebcb-139">Описание</span><span class="sxs-lookup"><span data-stu-id="cebcb-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cebcb-140">address</span><span class="sxs-lookup"><span data-stu-id="cebcb-140">address</span></span>|<span data-ttu-id="cebcb-141">string</span><span class="sxs-lookup"><span data-stu-id="cebcb-141">string</span></span>|<span data-ttu-id="cebcb-p108">Адрес или имя объекта range, представляющего источник данных. Если адрес не содержит имя листа, используется текущий активный лист.</span><span class="sxs-lookup"><span data-stu-id="cebcb-p108">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="cebcb-144">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="cebcb-144">hasHeaders</span></span>|<span data-ttu-id="cebcb-145">boolean</span><span class="sxs-lookup"><span data-stu-id="cebcb-145">boolean</span></span>|<span data-ttu-id="cebcb-p109">Логическое значение, указывающее, имеют ли импортируемые данные метки столбцов. Если источник не содержит заголовков (например, если этому свойству присвоено значение false), Excel автоматически создаст заголовок и сдвинет данные на одну строку вниз.</span><span class="sxs-lookup"><span data-stu-id="cebcb-p109">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="cebcb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="cebcb-149">Response</span></span>

<span data-ttu-id="cebcb-150">В случае успеха этот метод возвращает код ответа `200 OK` и объект [Table](../resources/table.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cebcb-150">If successful, this method returns `200 OK` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cebcb-151">Пример</span><span class="sxs-lookup"><span data-stu-id="cebcb-151">Example</span></span>
<span data-ttu-id="cebcb-152">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cebcb-152">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cebcb-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="cebcb-153">Request</span></span>
<span data-ttu-id="cebcb-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cebcb-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="cebcb-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="cebcb-155">Response</span></span>
<span data-ttu-id="cebcb-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cebcb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
