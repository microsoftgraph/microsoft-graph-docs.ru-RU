---
title: 'workbookPivotTable: refresh'
description: Обновляет сводную таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3238f67fc7f017e64ab327619a4f4f90fba71d1f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970782"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="e5a9b-103">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="e5a9b-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="e5a9b-104">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="e5a9b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5a9b-105">Permissions</span></span>
<span data-ttu-id="e5a9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5a9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e5a9b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5a9b-108">Permission type</span></span>      | <span data-ttu-id="e5a9b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5a9b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5a9b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5a9b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5a9b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5a9b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e5a9b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5a9b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5a9b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-113">Not supported.</span></span>    |
|<span data-ttu-id="e5a9b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5a9b-114">Application</span></span> | <span data-ttu-id="e5a9b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5a9b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5a9b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="e5a9b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5a9b-117">Request headers</span></span>
| <span data-ttu-id="e5a9b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e5a9b-118">Name</span></span>       | <span data-ttu-id="e5a9b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e5a9b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e5a9b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5a9b-120">Authorization</span></span>  | <span data-ttu-id="e5a9b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5a9b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e5a9b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e5a9b-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5a9b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5a9b-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="e5a9b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5a9b-127">Response</span></span>
<span data-ttu-id="e5a9b-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5a9b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e5a9b-130">Example</span></span>
<span data-ttu-id="e5a9b-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e5a9b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5a9b-132">Request</span></span>
<span data-ttu-id="e5a9b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="e5a9b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5a9b-134">Response</span></span>
<span data-ttu-id="e5a9b-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5a9b-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
