---
title: 'TableSort: apply'
description: Выполняет сортировку.
author: lumine2008
ms.openlocfilehash: d3e19dbd1ed77f32a215dfa165ebc796706b09a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309683"
---
# <a name="tablesort-apply"></a><span data-ttu-id="44912-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="44912-103">TableSort: apply</span></span>

<span data-ttu-id="44912-104">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="44912-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="44912-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44912-105">Permissions</span></span>
<span data-ttu-id="44912-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44912-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44912-108">Permission type</span></span>      | <span data-ttu-id="44912-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44912-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44912-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44912-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44912-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44912-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44912-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44912-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44912-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44912-113">Not supported.</span></span>    |
|<span data-ttu-id="44912-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44912-114">Application</span></span> | <span data-ttu-id="44912-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44912-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44912-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44912-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="44912-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44912-117">Request headers</span></span>
| <span data-ttu-id="44912-118">Имя</span><span class="sxs-lookup"><span data-stu-id="44912-118">Name</span></span>       | <span data-ttu-id="44912-119">Описание</span><span class="sxs-lookup"><span data-stu-id="44912-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44912-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44912-120">Authorization</span></span>  | <span data-ttu-id="44912-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44912-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44912-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="44912-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="44912-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="44912-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44912-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44912-126">Request body</span></span>
<span data-ttu-id="44912-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="44912-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="44912-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="44912-128">Parameter</span></span>    | <span data-ttu-id="44912-129">Тип</span><span class="sxs-lookup"><span data-stu-id="44912-129">Type</span></span>   |<span data-ttu-id="44912-130">Описание</span><span class="sxs-lookup"><span data-stu-id="44912-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44912-131">fields</span><span class="sxs-lookup"><span data-stu-id="44912-131">fields</span></span>|<span data-ttu-id="44912-132">WorkbookSortField коллекции</span><span class="sxs-lookup"><span data-stu-id="44912-132">WorkbookSortField collection</span></span>|<span data-ttu-id="44912-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="44912-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="44912-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="44912-134">matchCase</span></span>|<span data-ttu-id="44912-135">boolean</span><span class="sxs-lookup"><span data-stu-id="44912-135">boolean</span></span>|<span data-ttu-id="44912-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="44912-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="44912-138">method</span><span class="sxs-lookup"><span data-stu-id="44912-138">method</span></span>|<span data-ttu-id="44912-139">string</span><span class="sxs-lookup"><span data-stu-id="44912-139">string</span></span>|<span data-ttu-id="44912-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="44912-140">Optional.</span></span> <span data-ttu-id="44912-141">Метода упорядочения, используемый для китайских знаков.</span><span class="sxs-lookup"><span data-stu-id="44912-141">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="44912-142">Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="44912-142">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="44912-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="44912-143">Response</span></span>

<span data-ttu-id="44912-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="44912-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44912-146">Пример</span><span class="sxs-lookup"><span data-stu-id="44912-146">Example</span></span>
<span data-ttu-id="44912-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="44912-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="44912-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="44912-148">Request</span></span>
<span data-ttu-id="44912-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44912-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply
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

##### <a name="response"></a><span data-ttu-id="44912-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="44912-150">Response</span></span>
<span data-ttu-id="44912-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44912-151">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->