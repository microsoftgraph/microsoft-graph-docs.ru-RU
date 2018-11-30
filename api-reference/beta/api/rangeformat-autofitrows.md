---
title: 'RangeFormat: autofitRows'
description: Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.
ms.openlocfilehash: 428e405cad1464fad6e1e90940d9f9016fafdb48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077053"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="2d031-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="2d031-103">RangeFormat: autofitRows</span></span>

> <span data-ttu-id="2d031-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2d031-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d031-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d031-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d031-106">Изменяет высоту строк текущего диапазона так, чтобы она была оптимальной, с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="2d031-106">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d031-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d031-107">Permissions</span></span>
<span data-ttu-id="2d031-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d031-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d031-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d031-110">Permission type</span></span>      | <span data-ttu-id="2d031-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d031-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d031-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d031-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d031-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d031-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d031-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d031-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d031-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d031-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d031-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d031-116">Application</span></span> | <span data-ttu-id="2d031-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d031-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d031-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d031-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="2d031-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d031-119">Request headers</span></span>
| <span data-ttu-id="2d031-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2d031-120">Name</span></span>       | <span data-ttu-id="2d031-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2d031-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2d031-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d031-122">Authorization</span></span>  | <span data-ttu-id="2d031-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d031-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d031-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2d031-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2d031-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="2d031-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d031-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d031-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2d031-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d031-129">Response</span></span>

<span data-ttu-id="2d031-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2d031-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d031-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2d031-132">Example</span></span>
<span data-ttu-id="2d031-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2d031-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d031-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d031-134">Request</span></span>
<span data-ttu-id="2d031-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d031-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="2d031-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d031-136">Response</span></span>
<span data-ttu-id="2d031-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d031-137">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->