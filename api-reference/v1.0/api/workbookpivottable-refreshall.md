---
title: 'workbookPivotTable: refreshAll'
description: Обновляет сводную таблицу на заданном листе.
author: lumine2008
ms.openlocfilehash: dc94e5841440ba5110d7382abb04920e2d91015d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337914"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="dcb6c-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="dcb6c-103">workbookPivotTable: refreshAll</span></span>

<span data-ttu-id="dcb6c-104">Обновляет сводную таблицу на заданном листе.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcb6c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcb6c-105">Permissions</span></span>
<span data-ttu-id="dcb6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcb6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcb6c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcb6c-108">Permission type</span></span>      | <span data-ttu-id="dcb6c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcb6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcb6c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcb6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dcb6c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dcb6c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dcb6c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcb6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcb6c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-113">Not supported.</span></span>    |
|<span data-ttu-id="dcb6c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcb6c-114">Application</span></span> | <span data-ttu-id="dcb6c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcb6c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcb6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="dcb6c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcb6c-117">Request headers</span></span>
| <span data-ttu-id="dcb6c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dcb6c-118">Name</span></span>       | <span data-ttu-id="dcb6c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb6c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dcb6c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcb6c-120">Authorization</span></span>  | <span data-ttu-id="dcb6c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcb6c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dcb6c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="dcb6c-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcb6c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dcb6c-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="dcb6c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcb6c-127">Response</span></span>
<span data-ttu-id="dcb6c-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcb6c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dcb6c-130">Example</span></span>
<span data-ttu-id="dcb6c-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dcb6c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcb6c-132">Request</span></span>
<span data-ttu-id="dcb6c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="dcb6c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="dcb6c-134">Response</span></span>
<span data-ttu-id="dcb6c-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcb6c-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
