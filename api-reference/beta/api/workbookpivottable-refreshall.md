---
title: 'workbookPivotTable: refreshAll'
description: Обновляет сводную таблицу на заданном листе.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6edad0def37d67dddb6258814c6d4a4004a93366
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982241"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="50791-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="50791-103">workbookPivotTable: refreshAll</span></span>

> <span data-ttu-id="50791-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50791-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50791-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50791-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50791-106">Обновляет сводную таблицу на заданном листе.</span><span class="sxs-lookup"><span data-stu-id="50791-106">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="50791-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50791-107">Permissions</span></span>
<span data-ttu-id="50791-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50791-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50791-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50791-110">Permission type</span></span>      | <span data-ttu-id="50791-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50791-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50791-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50791-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50791-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50791-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50791-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50791-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50791-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50791-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="50791-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50791-116">Application</span></span> | <span data-ttu-id="50791-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50791-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50791-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50791-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="50791-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50791-119">Request headers</span></span>
| <span data-ttu-id="50791-120">Имя</span><span class="sxs-lookup"><span data-stu-id="50791-120">Name</span></span>       | <span data-ttu-id="50791-121">Описание</span><span class="sxs-lookup"><span data-stu-id="50791-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="50791-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50791-122">Authorization</span></span>  | <span data-ttu-id="50791-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50791-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50791-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="50791-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="50791-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="50791-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50791-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50791-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="50791-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="50791-129">Response</span></span>

<span data-ttu-id="50791-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="50791-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50791-132">Пример</span><span class="sxs-lookup"><span data-stu-id="50791-132">Example</span></span>
<span data-ttu-id="50791-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="50791-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="50791-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="50791-134">Request</span></span>
<span data-ttu-id="50791-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50791-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="50791-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="50791-136">Response</span></span>
<span data-ttu-id="50791-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="50791-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
