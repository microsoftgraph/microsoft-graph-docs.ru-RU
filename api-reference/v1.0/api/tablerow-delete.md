---
title: 'TableRow: delete'
description: Удаляет строку из таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f8b9139ac4eed6c2acbd68063ddb2b10021196fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024359"
---
# <a name="tablerow-delete"></a><span data-ttu-id="707ba-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="707ba-103">TableRow: delete</span></span>

<span data-ttu-id="707ba-104">Удаляет строку из таблицы.</span><span class="sxs-lookup"><span data-stu-id="707ba-104">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="707ba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="707ba-105">Permissions</span></span>
<span data-ttu-id="707ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="707ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="707ba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="707ba-108">Permission type</span></span>      | <span data-ttu-id="707ba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="707ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="707ba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="707ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="707ba-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="707ba-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="707ba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="707ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="707ba-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="707ba-113">Not supported.</span></span>    |
|<span data-ttu-id="707ba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="707ba-114">Application</span></span> | <span data-ttu-id="707ba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="707ba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="707ba-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="707ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/{index}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/delete

```
## <a name="request-headers"></a><span data-ttu-id="707ba-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="707ba-117">Request headers</span></span>
| <span data-ttu-id="707ba-118">Имя</span><span class="sxs-lookup"><span data-stu-id="707ba-118">Name</span></span>       | <span data-ttu-id="707ba-119">Описание</span><span class="sxs-lookup"><span data-stu-id="707ba-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="707ba-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="707ba-120">Authorization</span></span>  | <span data-ttu-id="707ba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="707ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="707ba-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="707ba-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="707ba-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="707ba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="707ba-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="707ba-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="707ba-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="707ba-127">Response</span></span>

<span data-ttu-id="707ba-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="707ba-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="707ba-130">Пример</span><span class="sxs-lookup"><span data-stu-id="707ba-130">Example</span></span>
<span data-ttu-id="707ba-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="707ba-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="707ba-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="707ba-132">Request</span></span>
<span data-ttu-id="707ba-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="707ba-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/delete
```

##### <a name="response"></a><span data-ttu-id="707ba-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="707ba-134">Response</span></span>
<span data-ttu-id="707ba-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="707ba-135">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
