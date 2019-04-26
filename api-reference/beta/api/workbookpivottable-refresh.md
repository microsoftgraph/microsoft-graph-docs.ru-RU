---
title: 'workbookPivotTable: refresh'
description: Обновляет сводную таблицу.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: aefdbc3368c9831d9b0487659ef7bb1d347da6e9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339644"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="d85cd-103">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="d85cd-103">workbookPivotTable: refresh</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d85cd-104">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="d85cd-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="d85cd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d85cd-105">Permissions</span></span>
<span data-ttu-id="d85cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d85cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d85cd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d85cd-108">Permission type</span></span>      | <span data-ttu-id="d85cd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d85cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d85cd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d85cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d85cd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d85cd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d85cd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d85cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d85cd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d85cd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d85cd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d85cd-114">Application</span></span> | <span data-ttu-id="d85cd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d85cd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d85cd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d85cd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="d85cd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d85cd-117">Request headers</span></span>
| <span data-ttu-id="d85cd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d85cd-118">Name</span></span>       | <span data-ttu-id="d85cd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d85cd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d85cd-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d85cd-120">Authorization</span></span>  | <span data-ttu-id="d85cd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d85cd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d85cd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d85cd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d85cd-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d85cd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d85cd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d85cd-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d85cd-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d85cd-127">Response</span></span>

<span data-ttu-id="d85cd-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d85cd-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d85cd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d85cd-130">Example</span></span>
<span data-ttu-id="d85cd-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d85cd-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d85cd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d85cd-132">Request</span></span>
<span data-ttu-id="d85cd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d85cd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="d85cd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d85cd-134">Response</span></span>
<span data-ttu-id="d85cd-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d85cd-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
