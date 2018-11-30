---
title: 'TableRow: delete'
description: Удаляет строку из таблицы.
ms.openlocfilehash: a2202daf9a645a16a7ea6287edf468e12d829e9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080333"
---
# <a name="tablerow-delete"></a><span data-ttu-id="833df-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="833df-103">TableRow: delete</span></span>

> <span data-ttu-id="833df-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="833df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="833df-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="833df-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="833df-106">Удаляет строку из таблицы.</span><span class="sxs-lookup"><span data-stu-id="833df-106">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="833df-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="833df-107">Permissions</span></span>
<span data-ttu-id="833df-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="833df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="833df-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="833df-110">Permission type</span></span>      | <span data-ttu-id="833df-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="833df-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="833df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="833df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="833df-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="833df-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="833df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="833df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="833df-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="833df-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="833df-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="833df-116">Application</span></span> | <span data-ttu-id="833df-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="833df-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="833df-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="833df-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="833df-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="833df-119">Request headers</span></span>
| <span data-ttu-id="833df-120">Имя</span><span class="sxs-lookup"><span data-stu-id="833df-120">Name</span></span>       | <span data-ttu-id="833df-121">Описание</span><span class="sxs-lookup"><span data-stu-id="833df-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="833df-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="833df-122">Authorization</span></span>  | <span data-ttu-id="833df-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="833df-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="833df-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="833df-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="833df-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="833df-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="833df-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="833df-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="833df-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="833df-129">Response</span></span>

<span data-ttu-id="833df-p105">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="833df-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="833df-132">Пример</span><span class="sxs-lookup"><span data-stu-id="833df-132">Example</span></span>
<span data-ttu-id="833df-133">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="833df-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="833df-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="833df-134">Request</span></span>
<span data-ttu-id="833df-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="833df-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/delete
```

##### <a name="response"></a><span data-ttu-id="833df-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="833df-136">Response</span></span>
<span data-ttu-id="833df-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="833df-137">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->