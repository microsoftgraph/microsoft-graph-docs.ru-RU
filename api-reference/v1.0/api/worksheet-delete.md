---
title: 'Worksheet: delete'
description: Удаляет лист из книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: ee46051e611866c3e18d72396762276eb22f52e7
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515781"
---
# <a name="worksheet-delete"></a><span data-ttu-id="a4a21-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="a4a21-103">Worksheet: delete</span></span>

<span data-ttu-id="a4a21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4a21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4a21-105">Удаляет лист из книги.</span><span class="sxs-lookup"><span data-stu-id="a4a21-105">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4a21-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4a21-106">Permissions</span></span>
<span data-ttu-id="a4a21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4a21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4a21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4a21-109">Permission type</span></span>      | <span data-ttu-id="a4a21-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4a21-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4a21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4a21-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4a21-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4a21-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a4a21-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4a21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4a21-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4a21-114">Not supported.</span></span>    |
|<span data-ttu-id="a4a21-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4a21-115">Application</span></span> | <span data-ttu-id="a4a21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4a21-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4a21-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4a21-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /workbook/worksheets/{id|name}

```
## <a name="request-headers"></a><span data-ttu-id="a4a21-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4a21-118">Request headers</span></span>
| <span data-ttu-id="a4a21-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a4a21-119">Name</span></span>       | <span data-ttu-id="a4a21-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a4a21-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4a21-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4a21-121">Authorization</span></span>  | <span data-ttu-id="a4a21-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4a21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4a21-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a4a21-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="a4a21-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="a4a21-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4a21-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4a21-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a4a21-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4a21-128">Response</span></span>

<span data-ttu-id="a4a21-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a4a21-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4a21-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a4a21-131">Example</span></span>
<span data-ttu-id="a4a21-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a4a21-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a4a21-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4a21-133">Request</span></span>
<span data-ttu-id="a4a21-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4a21-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
```

##### <a name="response"></a><span data-ttu-id="a4a21-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4a21-135">Response</span></span>
<span data-ttu-id="a4a21-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a4a21-136">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

