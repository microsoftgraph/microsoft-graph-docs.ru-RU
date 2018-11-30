---
title: Обновление таблицы
description: Обновление свойств объекта таблицы.
ms.openlocfilehash: a929329ed9a88b7dda6206193292f1ca1e63ced1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077987"
---
# <a name="update-table"></a><span data-ttu-id="4a788-103">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="4a788-103">Update table</span></span>

> <span data-ttu-id="4a788-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4a788-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a788-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a788-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a788-106">Обновление свойств объекта таблицы.</span><span class="sxs-lookup"><span data-stu-id="4a788-106">Update the properties of table object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a788-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a788-107">Permissions</span></span>
<span data-ttu-id="4a788-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a788-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a788-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a788-110">Permission type</span></span>      | <span data-ttu-id="4a788-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a788-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a788-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a788-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a788-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a788-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a788-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a788-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a788-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a788-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a788-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a788-116">Application</span></span> | <span data-ttu-id="4a788-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a788-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a788-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a788-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}
PATCH /workbook/worksheets/{id|name}/tables/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4a788-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a788-119">Optional request headers</span></span>
| <span data-ttu-id="4a788-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4a788-120">Name</span></span>       | <span data-ttu-id="4a788-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4a788-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4a788-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a788-122">Authorization</span></span>  | <span data-ttu-id="4a788-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a788-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a788-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4a788-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4a788-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4a788-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a788-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a788-128">Request body</span></span>
<span data-ttu-id="4a788-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4a788-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4a788-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a788-132">Property</span></span>     | <span data-ttu-id="4a788-133">Тип</span><span class="sxs-lookup"><span data-stu-id="4a788-133">Type</span></span>   |<span data-ttu-id="4a788-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4a788-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a788-135">name</span><span class="sxs-lookup"><span data-stu-id="4a788-135">name</span></span>|<span data-ttu-id="4a788-136">строка</span><span class="sxs-lookup"><span data-stu-id="4a788-136">string</span></span>|<span data-ttu-id="4a788-137">Имя таблицы.</span><span class="sxs-lookup"><span data-stu-id="4a788-137">Name of the table.</span></span>|
|<span data-ttu-id="4a788-138">showHeaders</span><span class="sxs-lookup"><span data-stu-id="4a788-138">showHeaders</span></span>|<span data-ttu-id="4a788-139">boolean</span><span class="sxs-lookup"><span data-stu-id="4a788-139">boolean</span></span>|<span data-ttu-id="4a788-p106">Указывает, отображается ли строка заголовков. Можно задать это значение, чтобы отобразить или скрыть строку заголовков.</span><span class="sxs-lookup"><span data-stu-id="4a788-p106">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="4a788-142">showTotals</span><span class="sxs-lookup"><span data-stu-id="4a788-142">showTotals</span></span>|<span data-ttu-id="4a788-143">boolean</span><span class="sxs-lookup"><span data-stu-id="4a788-143">boolean</span></span>|<span data-ttu-id="4a788-p107">Указывает, отображается ли строка итогов. Можно задать это значение, чтобы отобразить или скрыть строку итогов.</span><span class="sxs-lookup"><span data-stu-id="4a788-p107">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="4a788-146">style</span><span class="sxs-lookup"><span data-stu-id="4a788-146">style</span></span>|<span data-ttu-id="4a788-147">строка</span><span class="sxs-lookup"><span data-stu-id="4a788-147">string</span></span>|<span data-ttu-id="4a788-p108">Постоянное значение, представляющее стиль таблицы. Возможные значения: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. Также можно указать настраиваемый пользовательский стиль, имеющийся в книге.</span><span class="sxs-lookup"><span data-stu-id="4a788-p108">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="4a788-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a788-151">Response</span></span>

<span data-ttu-id="4a788-152">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [Table](../resources/table.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a788-152">If successful, this method returns a `200 OK` response code and updated [Table](../resources/table.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a788-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4a788-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a788-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a788-154">Request</span></span>
<span data-ttu-id="4a788-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a788-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_table"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}
Content-type: application/json
Content-length: 109

{
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
##### <a name="response"></a><span data-ttu-id="4a788-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a788-156">Response</span></span>
<span data-ttu-id="4a788-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4a788-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
