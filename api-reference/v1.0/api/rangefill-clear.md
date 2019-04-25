---
title: 'RangeFill: clear'
description: Сбрасывает фон диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 53871f65eb3dd5b9f3464458265fd0019137d95d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582334"
---
# <a name="rangefill-clear"></a><span data-ttu-id="9c03d-103">RangeFill: clear</span><span class="sxs-lookup"><span data-stu-id="9c03d-103">RangeFill: clear</span></span>

<span data-ttu-id="9c03d-104">Сбрасывает фон диапазона.</span><span class="sxs-lookup"><span data-stu-id="9c03d-104">Resets the range background.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c03d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c03d-105">Permissions</span></span>
<span data-ttu-id="9c03d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c03d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c03d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c03d-108">Permission type</span></span>      | <span data-ttu-id="9c03d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c03d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c03d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c03d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c03d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c03d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9c03d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c03d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c03d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c03d-113">Not supported.</span></span>    |
|<span data-ttu-id="9c03d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c03d-114">Application</span></span> | <span data-ttu-id="9c03d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c03d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c03d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c03d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/fill/clear
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/fill/clear
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="9c03d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c03d-117">Request headers</span></span>
| <span data-ttu-id="9c03d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9c03d-118">Name</span></span>       | <span data-ttu-id="9c03d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9c03d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9c03d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c03d-120">Authorization</span></span>  | <span data-ttu-id="9c03d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c03d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c03d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9c03d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9c03d-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9c03d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c03d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c03d-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9c03d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c03d-127">Response</span></span>

<span data-ttu-id="9c03d-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9c03d-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c03d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9c03d-130">Example</span></span>
<span data-ttu-id="9c03d-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9c03d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9c03d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c03d-132">Request</span></span>
<span data-ttu-id="9c03d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c03d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangefill_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="9c03d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c03d-134">Response</span></span>
<span data-ttu-id="9c03d-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c03d-135">Here is an example of the response.</span></span> 
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
  "description": "RangeFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
