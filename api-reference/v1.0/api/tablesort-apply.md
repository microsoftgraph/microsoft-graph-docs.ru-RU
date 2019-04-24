---
title: 'TableSort: apply'
description: Выполнение сортировки.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 69fda9b0a49c59a86a17e9a41eb89159085d857e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520244"
---
# <a name="tablesort-apply"></a><span data-ttu-id="83469-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="83469-103">TableSort: apply</span></span>

<span data-ttu-id="83469-104">Выполнение сортировки.</span><span class="sxs-lookup"><span data-stu-id="83469-104">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="83469-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83469-105">Permissions</span></span>
<span data-ttu-id="83469-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83469-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83469-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83469-108">Permission type</span></span>      | <span data-ttu-id="83469-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83469-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83469-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83469-110">Delegated (work or school account)</span></span> | <span data-ttu-id="83469-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83469-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="83469-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83469-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83469-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83469-113">Not supported.</span></span>    |
|<span data-ttu-id="83469-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83469-114">Application</span></span> | <span data-ttu-id="83469-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83469-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83469-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83469-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="83469-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83469-117">Request headers</span></span>
| <span data-ttu-id="83469-118">Имя</span><span class="sxs-lookup"><span data-stu-id="83469-118">Name</span></span>       | <span data-ttu-id="83469-119">Описание</span><span class="sxs-lookup"><span data-stu-id="83469-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="83469-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83469-120">Authorization</span></span>  | <span data-ttu-id="83469-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83469-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83469-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="83469-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="83469-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="83469-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83469-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83469-126">Request body</span></span>
<span data-ttu-id="83469-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="83469-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="83469-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="83469-128">Parameter</span></span>    | <span data-ttu-id="83469-129">Тип</span><span class="sxs-lookup"><span data-stu-id="83469-129">Type</span></span>   |<span data-ttu-id="83469-130">Описание</span><span class="sxs-lookup"><span data-stu-id="83469-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83469-131">fields</span><span class="sxs-lookup"><span data-stu-id="83469-131">fields</span></span>|<span data-ttu-id="83469-132">Коллекция Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="83469-132">WorkbookSortField collection</span></span>|<span data-ttu-id="83469-133">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="83469-133">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="83469-134">matchCase</span><span class="sxs-lookup"><span data-stu-id="83469-134">matchCase</span></span>|<span data-ttu-id="83469-135">boolean</span><span class="sxs-lookup"><span data-stu-id="83469-135">boolean</span></span>|<span data-ttu-id="83469-p104">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="83469-p104">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="83469-138">method</span><span class="sxs-lookup"><span data-stu-id="83469-138">method</span></span>|<span data-ttu-id="83469-139">string</span><span class="sxs-lookup"><span data-stu-id="83469-139">string</span></span>|<span data-ttu-id="83469-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="83469-140">Optional.</span></span> <span data-ttu-id="83469-141">Метод сортировки, используемый для китайских символов.</span><span class="sxs-lookup"><span data-stu-id="83469-141">The ordering method used for Chinese characters.</span></span>  <span data-ttu-id="83469-142">Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="83469-142">The possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="83469-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="83469-143">Response</span></span>

<span data-ttu-id="83469-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="83469-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83469-146">Пример</span><span class="sxs-lookup"><span data-stu-id="83469-146">Example</span></span>
<span data-ttu-id="83469-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="83469-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="83469-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="83469-148">Request</span></span>
<span data-ttu-id="83469-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83469-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="83469-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="83469-150">Response</span></span>
<span data-ttu-id="83469-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="83469-151">Here is an example of the response.</span></span> 
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
