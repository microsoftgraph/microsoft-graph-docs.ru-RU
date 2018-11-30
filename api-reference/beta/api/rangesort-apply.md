---
title: 'RangeSort: apply'
description: Выполнение операции сортировки.
ms.openlocfilehash: d5547d59f662875c018c7e2c2db1074d6d197be2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079059"
---
# <a name="rangesort-apply"></a><span data-ttu-id="4e02c-103">RangeSort: apply</span><span class="sxs-lookup"><span data-stu-id="4e02c-103">RangeSort: apply</span></span>

> <span data-ttu-id="4e02c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4e02c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e02c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e02c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e02c-106">Выполнение операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="4e02c-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="4e02c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e02c-107">Permissions</span></span>
<span data-ttu-id="4e02c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e02c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e02c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e02c-110">Permission type</span></span>      | <span data-ttu-id="4e02c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e02c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e02c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e02c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e02c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e02c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e02c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e02c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e02c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e02c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4e02c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e02c-116">Application</span></span> | <span data-ttu-id="4e02c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e02c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e02c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e02c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/sort/apply
POST /workbook/worksheets/{id|name}/range(address='<address>')/sort/apply
POST /workbook/tables/{id|name}/columns/{id|name}/range/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="4e02c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e02c-119">Request headers</span></span>
| <span data-ttu-id="4e02c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4e02c-120">Name</span></span>       | <span data-ttu-id="4e02c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4e02c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4e02c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e02c-122">Authorization</span></span>  | <span data-ttu-id="4e02c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e02c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e02c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4e02c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4e02c-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e02c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e02c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e02c-128">Request body</span></span>
<span data-ttu-id="4e02c-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4e02c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4e02c-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="4e02c-130">Parameter</span></span>    | <span data-ttu-id="4e02c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e02c-131">Type</span></span>   |<span data-ttu-id="4e02c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e02c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e02c-133">fields</span><span class="sxs-lookup"><span data-stu-id="4e02c-133">fields</span></span>|<span data-ttu-id="4e02c-134">SortField</span><span class="sxs-lookup"><span data-stu-id="4e02c-134">SortField</span></span>|<span data-ttu-id="4e02c-135">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="4e02c-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="4e02c-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="4e02c-136">matchCase</span></span>|<span data-ttu-id="4e02c-137">boolean</span><span class="sxs-lookup"><span data-stu-id="4e02c-137">boolean</span></span>|<span data-ttu-id="4e02c-p105">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="4e02c-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="4e02c-140">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="4e02c-140">hasHeaders</span></span>|<span data-ttu-id="4e02c-141">boolean</span><span class="sxs-lookup"><span data-stu-id="4e02c-141">boolean</span></span>|<span data-ttu-id="4e02c-p106">Необязательный параметр. Указывает, есть ли у диапазона заголовок.</span><span class="sxs-lookup"><span data-stu-id="4e02c-p106">Optional. Whether the range has a header.</span></span>|
|<span data-ttu-id="4e02c-144">orientation</span><span class="sxs-lookup"><span data-stu-id="4e02c-144">orientation</span></span>|<span data-ttu-id="4e02c-145">string</span><span class="sxs-lookup"><span data-stu-id="4e02c-145">string</span></span>|<span data-ttu-id="4e02c-p107">Необязательный параметр. Указывает направление сортировки: по строкам или по столбцам.  Возможные значения: `Rows`, `Columns`.</span><span class="sxs-lookup"><span data-stu-id="4e02c-p107">Optional. Whether the operation is sorting rows or columns.  Possible values are: `Rows`, `Columns`.</span></span>|
|<span data-ttu-id="4e02c-149">метод</span><span class="sxs-lookup"><span data-stu-id="4e02c-149">method</span></span>|<span data-ttu-id="4e02c-150">string</span><span class="sxs-lookup"><span data-stu-id="4e02c-150">string</span></span>|<span data-ttu-id="4e02c-p108">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="4e02c-p108">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="4e02c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e02c-154">Response</span></span>

<span data-ttu-id="4e02c-p109">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4e02c-p109">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e02c-157">Пример</span><span class="sxs-lookup"><span data-stu-id="4e02c-157">Example</span></span>
<span data-ttu-id="4e02c-158">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4e02c-158">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4e02c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e02c-159">Request</span></span>
<span data-ttu-id="4e02c-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e02c-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
Content-type: application/json
Content-length: 358

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
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <a name="response"></a><span data-ttu-id="4e02c-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e02c-161">Response</span></span>
<span data-ttu-id="4e02c-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e02c-162">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->