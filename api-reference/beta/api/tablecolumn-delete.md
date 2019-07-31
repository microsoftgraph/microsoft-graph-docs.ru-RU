---
title: 'TableColumn: delete'
description: Удаляет столбец из таблицы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3fac49c7f11123f9f0435762b053b47438f5bbdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982538"
---
# <a name="tablecolumn-delete"></a><span data-ttu-id="bfc81-103">TableColumn: delete</span><span class="sxs-lookup"><span data-stu-id="bfc81-103">TableColumn: delete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfc81-104">Удаляет столбец из таблицы.</span><span class="sxs-lookup"><span data-stu-id="bfc81-104">Deletes the column from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfc81-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfc81-105">Permissions</span></span>
<span data-ttu-id="bfc81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfc81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfc81-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfc81-108">Permission type</span></span>      | <span data-ttu-id="bfc81-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfc81-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfc81-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfc81-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfc81-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfc81-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bfc81-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfc81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfc81-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfc81-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bfc81-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfc81-114">Application</span></span> | <span data-ttu-id="bfc81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfc81-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfc81-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfc81-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="bfc81-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfc81-117">Request headers</span></span>
| <span data-ttu-id="bfc81-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bfc81-118">Name</span></span>       | <span data-ttu-id="bfc81-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bfc81-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bfc81-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfc81-120">Authorization</span></span>  | <span data-ttu-id="bfc81-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfc81-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfc81-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bfc81-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bfc81-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="bfc81-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfc81-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfc81-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bfc81-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfc81-127">Response</span></span>

<span data-ttu-id="bfc81-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bfc81-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfc81-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bfc81-130">Example</span></span>
<span data-ttu-id="bfc81-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="bfc81-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bfc81-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfc81-132">Request</span></span>
<span data-ttu-id="bfc81-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfc81-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="bfc81-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfc81-134">Response</span></span>
<span data-ttu-id="bfc81-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bfc81-135">Here is an example of the response.</span></span> 
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
  "description": "TableColumn: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
