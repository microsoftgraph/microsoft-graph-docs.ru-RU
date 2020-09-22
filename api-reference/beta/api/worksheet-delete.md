---
title: 'Worksheet: delete'
description: Удаляет лист из книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 47292fbffad4902acb7433a40ffadf4681140423
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092902"
---
# <a name="worksheet-delete"></a><span data-ttu-id="b2e40-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="b2e40-103">Worksheet: delete</span></span>

<span data-ttu-id="b2e40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2e40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2e40-105">Удаляет лист из книги.</span><span class="sxs-lookup"><span data-stu-id="b2e40-105">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="b2e40-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2e40-106">Permissions</span></span>
<span data-ttu-id="b2e40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2e40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2e40-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2e40-109">Permission type</span></span>      | <span data-ttu-id="b2e40-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2e40-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2e40-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2e40-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b2e40-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2e40-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2e40-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2e40-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2e40-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2e40-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b2e40-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2e40-115">Application</span></span> | <span data-ttu-id="b2e40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e40-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2e40-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2e40-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="b2e40-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2e40-118">Request headers</span></span>
| <span data-ttu-id="b2e40-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b2e40-119">Name</span></span>       | <span data-ttu-id="b2e40-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e40-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2e40-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2e40-121">Authorization</span></span>  | <span data-ttu-id="b2e40-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2e40-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2e40-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b2e40-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="b2e40-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="b2e40-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2e40-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2e40-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b2e40-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2e40-128">Response</span></span>

<span data-ttu-id="b2e40-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b2e40-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2e40-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b2e40-131">Example</span></span>
<span data-ttu-id="b2e40-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b2e40-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b2e40-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2e40-133">Request</span></span>
<span data-ttu-id="b2e40-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2e40-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="b2e40-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2e40-135">Response</span></span>
<span data-ttu-id="b2e40-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b2e40-136">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


