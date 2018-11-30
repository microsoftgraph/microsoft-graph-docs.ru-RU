---
title: 'WorksheetProtection: unprotect'
description: Снятие защиты с листа
ms.openlocfilehash: 32909d81119c326172a12d346ea53d9f8eb2b71b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081333"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="9464e-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="9464e-103">WorksheetProtection: unprotect</span></span>

> <span data-ttu-id="9464e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9464e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9464e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9464e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9464e-106">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="9464e-106">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="9464e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9464e-107">Permissions</span></span>
<span data-ttu-id="9464e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9464e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9464e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9464e-110">Permission type</span></span>      | <span data-ttu-id="9464e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9464e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9464e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9464e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9464e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9464e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9464e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9464e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9464e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9464e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9464e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9464e-116">Application</span></span> | <span data-ttu-id="9464e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9464e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9464e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9464e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="9464e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9464e-119">Request headers</span></span>
| <span data-ttu-id="9464e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9464e-120">Name</span></span>       | <span data-ttu-id="9464e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9464e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9464e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9464e-122">Authorization</span></span>  | <span data-ttu-id="9464e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9464e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9464e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9464e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="9464e-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9464e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9464e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9464e-128">Request body</span></span>
<span data-ttu-id="9464e-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9464e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9464e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="9464e-130">Parameter</span></span>    | <span data-ttu-id="9464e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9464e-131">Type</span></span>   |<span data-ttu-id="9464e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9464e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9464e-133">password</span><span class="sxs-lookup"><span data-stu-id="9464e-133">password</span></span>|<span data-ttu-id="9464e-134">string</span><span class="sxs-lookup"><span data-stu-id="9464e-134">string</span></span>|<span data-ttu-id="9464e-p105">Необязательный пароль защиты листа.</span><span class="sxs-lookup"><span data-stu-id="9464e-p105">Optional. sheet protection password.</span></span>|

## <a name="response"></a><span data-ttu-id="9464e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9464e-137">Response</span></span>

<span data-ttu-id="9464e-p106">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9464e-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9464e-140">Пример</span><span class="sxs-lookup"><span data-stu-id="9464e-140">Example</span></span>
<span data-ttu-id="9464e-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9464e-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9464e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9464e-142">Request</span></span>
<span data-ttu-id="9464e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9464e-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <a name="response"></a><span data-ttu-id="9464e-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="9464e-144">Response</span></span>
<span data-ttu-id="9464e-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9464e-145">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->