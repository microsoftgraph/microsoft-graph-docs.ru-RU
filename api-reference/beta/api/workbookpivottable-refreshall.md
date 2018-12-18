---
title: 'workbookPivotTable: refreshAll'
description: Обновляет сводную таблицу на заданном листе.
author: lumine2008
ms.openlocfilehash: 08a4015d58e68a3099448be91537b7970d5c1ddd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308227"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="03e44-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="03e44-103">workbookPivotTable: refreshAll</span></span>

> <span data-ttu-id="03e44-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03e44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03e44-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e44-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03e44-106">Обновляет сводную таблицу на заданном листе.</span><span class="sxs-lookup"><span data-stu-id="03e44-106">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="03e44-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03e44-107">Permissions</span></span>
<span data-ttu-id="03e44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03e44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03e44-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03e44-110">Permission type</span></span>      | <span data-ttu-id="03e44-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03e44-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03e44-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03e44-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03e44-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03e44-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03e44-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03e44-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03e44-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03e44-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03e44-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03e44-116">Application</span></span> | <span data-ttu-id="03e44-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e44-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03e44-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03e44-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="03e44-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03e44-119">Request headers</span></span>
| <span data-ttu-id="03e44-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03e44-120">Name</span></span>       | <span data-ttu-id="03e44-121">Описание</span><span class="sxs-lookup"><span data-stu-id="03e44-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03e44-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03e44-122">Authorization</span></span>  | <span data-ttu-id="03e44-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03e44-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03e44-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="03e44-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="03e44-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="03e44-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03e44-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03e44-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="03e44-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="03e44-129">Response</span></span>

<span data-ttu-id="03e44-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="03e44-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e44-132">Пример</span><span class="sxs-lookup"><span data-stu-id="03e44-132">Example</span></span>
<span data-ttu-id="03e44-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="03e44-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03e44-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="03e44-134">Request</span></span>
<span data-ttu-id="03e44-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03e44-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="03e44-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="03e44-136">Response</span></span>
<span data-ttu-id="03e44-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03e44-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
