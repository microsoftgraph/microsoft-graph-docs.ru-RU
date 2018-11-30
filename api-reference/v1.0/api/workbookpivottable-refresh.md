---
title: 'workbookPivotTable: refresh'
description: Обновляет сводную таблицу.
ms.openlocfilehash: 3acbe6efb29d6846b48bfae250731640ad533dad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025555"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="6520d-103">workbookPivotTable: refresh</span><span class="sxs-lookup"><span data-stu-id="6520d-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="6520d-104">Обновляет сводную таблицу.</span><span class="sxs-lookup"><span data-stu-id="6520d-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="6520d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6520d-105">Permissions</span></span>
<span data-ttu-id="6520d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6520d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6520d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6520d-108">Permission type</span></span>      | <span data-ttu-id="6520d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6520d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6520d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6520d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6520d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6520d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6520d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6520d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6520d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6520d-113">Not supported.</span></span>    |
|<span data-ttu-id="6520d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6520d-114">Application</span></span> | <span data-ttu-id="6520d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6520d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6520d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6520d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="6520d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6520d-117">Request headers</span></span>
| <span data-ttu-id="6520d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6520d-118">Name</span></span>       | <span data-ttu-id="6520d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6520d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6520d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6520d-120">Authorization</span></span>  | <span data-ttu-id="6520d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6520d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6520d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6520d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6520d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6520d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6520d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6520d-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="6520d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6520d-127">Response</span></span>
<span data-ttu-id="6520d-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6520d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6520d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6520d-130">Example</span></span>
<span data-ttu-id="6520d-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6520d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6520d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6520d-132">Request</span></span>
<span data-ttu-id="6520d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6520d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="6520d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6520d-134">Response</span></span>
<span data-ttu-id="6520d-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6520d-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
