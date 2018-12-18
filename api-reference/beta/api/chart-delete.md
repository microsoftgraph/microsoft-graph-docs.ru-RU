---
title: 'Chart: delete'
description: Удаляет объект диаграммы.
author: lumine2008
ms.openlocfilehash: bb92d9f66bfcaed1d72e4d288d7bbc465f9aa2eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356548"
---
# <a name="chart-delete"></a><span data-ttu-id="c260f-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="c260f-103">Chart: delete</span></span>

> <span data-ttu-id="c260f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c260f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c260f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c260f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c260f-106">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c260f-106">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c260f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c260f-107">Permissions</span></span>
<span data-ttu-id="c260f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c260f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c260f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c260f-110">Permission type</span></span>      | <span data-ttu-id="c260f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c260f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c260f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c260f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c260f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c260f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c260f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c260f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c260f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c260f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c260f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c260f-116">Application</span></span> | <span data-ttu-id="c260f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c260f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c260f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c260f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts(<name>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="c260f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c260f-119">Request headers</span></span>
| <span data-ttu-id="c260f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c260f-120">Name</span></span>       | <span data-ttu-id="c260f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c260f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c260f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c260f-122">Authorization</span></span>  | <span data-ttu-id="c260f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c260f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c260f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c260f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c260f-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="c260f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c260f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c260f-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="c260f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c260f-129">Response</span></span>

<span data-ttu-id="c260f-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c260f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c260f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c260f-132">Example</span></span>
<span data-ttu-id="c260f-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c260f-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c260f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c260f-134">Request</span></span>
<span data-ttu-id="c260f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c260f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/delete
```

##### <a name="response"></a><span data-ttu-id="c260f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c260f-136">Response</span></span>
<span data-ttu-id="c260f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c260f-137">Here is an example of the response.</span></span> 
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
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->