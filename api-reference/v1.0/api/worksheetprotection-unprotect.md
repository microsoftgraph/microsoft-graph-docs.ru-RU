---
title: 'WorksheetProtection: unprotect'
description: Снятие защиты с листа
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 273f841a4fc05d78dece7ab26f233eb28c314a88
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813029"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="632f3-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="632f3-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="632f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="632f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="632f3-105">Снятие защиты с листа</span><span class="sxs-lookup"><span data-stu-id="632f3-105">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="632f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="632f3-106">Permissions</span></span>
<span data-ttu-id="632f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="632f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="632f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="632f3-109">Permission type</span></span>      | <span data-ttu-id="632f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="632f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="632f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="632f3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="632f3-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="632f3-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="632f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="632f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="632f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="632f3-114">Not supported.</span></span>    |
|<span data-ttu-id="632f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="632f3-115">Application</span></span> | <span data-ttu-id="632f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="632f3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="632f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="632f3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="632f3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="632f3-118">Request headers</span></span>
| <span data-ttu-id="632f3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="632f3-119">Name</span></span>       | <span data-ttu-id="632f3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="632f3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="632f3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="632f3-121">Authorization</span></span>  | <span data-ttu-id="632f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="632f3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="632f3-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="632f3-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="632f3-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="632f3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="632f3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="632f3-127">Request body</span></span>
<span data-ttu-id="632f3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="632f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="632f3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="632f3-129">Response</span></span>

<span data-ttu-id="632f3-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="632f3-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="632f3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="632f3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="632f3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="632f3-133">Request</span></span>
<span data-ttu-id="632f3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="632f3-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
```


### <a name="response"></a><span data-ttu-id="632f3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="632f3-135">Response</span></span>
<span data-ttu-id="632f3-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="632f3-136">The following is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

