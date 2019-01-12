---
title: 'TableSort: apply'
description: Выполняет сортировку.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f39108f0413917fcf1204f4c2fb6640094d25ced
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918408"
---
# <a name="tablesort-apply"></a><span data-ttu-id="14220-103">TableSort: apply</span><span class="sxs-lookup"><span data-stu-id="14220-103">TableSort: apply</span></span>

> <span data-ttu-id="14220-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14220-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14220-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14220-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14220-106">Выполнение операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="14220-106">Perform a sort operation.</span></span>
## <a name="permissions"></a><span data-ttu-id="14220-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14220-107">Permissions</span></span>
<span data-ttu-id="14220-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14220-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14220-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14220-110">Permission type</span></span>      | <span data-ttu-id="14220-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14220-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14220-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14220-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14220-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14220-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="14220-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14220-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14220-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14220-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="14220-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14220-116">Application</span></span> | <span data-ttu-id="14220-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14220-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14220-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14220-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/apply

```
## <a name="request-headers"></a><span data-ttu-id="14220-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14220-119">Request headers</span></span>
| <span data-ttu-id="14220-120">Имя</span><span class="sxs-lookup"><span data-stu-id="14220-120">Name</span></span>       | <span data-ttu-id="14220-121">Описание</span><span class="sxs-lookup"><span data-stu-id="14220-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="14220-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14220-122">Authorization</span></span>  | <span data-ttu-id="14220-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14220-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14220-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="14220-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="14220-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="14220-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14220-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14220-128">Request body</span></span>
<span data-ttu-id="14220-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="14220-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="14220-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="14220-130">Parameter</span></span>    | <span data-ttu-id="14220-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14220-131">Type</span></span>   |<span data-ttu-id="14220-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14220-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14220-133">fields</span><span class="sxs-lookup"><span data-stu-id="14220-133">fields</span></span>|<span data-ttu-id="14220-134">SortField</span><span class="sxs-lookup"><span data-stu-id="14220-134">SortField</span></span>|<span data-ttu-id="14220-135">Список условий для сортировки.</span><span class="sxs-lookup"><span data-stu-id="14220-135">The list of conditions to sort on.</span></span>|
|<span data-ttu-id="14220-136">matchCase</span><span class="sxs-lookup"><span data-stu-id="14220-136">matchCase</span></span>|<span data-ttu-id="14220-137">boolean</span><span class="sxs-lookup"><span data-stu-id="14220-137">boolean</span></span>|<span data-ttu-id="14220-p105">Необязательный. Указывает, необходимо ли учитывать регистр при сортировке строк.</span><span class="sxs-lookup"><span data-stu-id="14220-p105">Optional. Whether to have the casing impact string ordering.</span></span>|
|<span data-ttu-id="14220-140">method</span><span class="sxs-lookup"><span data-stu-id="14220-140">method</span></span>|<span data-ttu-id="14220-141">string</span><span class="sxs-lookup"><span data-stu-id="14220-141">string</span></span>|<span data-ttu-id="14220-p106">Необязательный параметр. Метод сортировки, используемый для китайских символов.  Возможные значения: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="14220-p106">Optional. The ordering method used for Chinese characters.  Possible values are: `PinYin`, `StrokeCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="14220-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="14220-145">Response</span></span>

<span data-ttu-id="14220-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="14220-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14220-148">Пример</span><span class="sxs-lookup"><span data-stu-id="14220-148">Example</span></span>
<span data-ttu-id="14220-149">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="14220-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="14220-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="14220-150">Request</span></span>
<span data-ttu-id="14220-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14220-151">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="14220-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="14220-152">Response</span></span>
<span data-ttu-id="14220-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14220-153">Here is an example of the response.</span></span> 
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
  "description": "TableSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
