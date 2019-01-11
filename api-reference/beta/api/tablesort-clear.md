---
title: 'TableSort: clear'
description: Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.
localization_priority: Normal
ms.openlocfilehash: 1d7d695bfc1d1e6d951f44e0e3e7cde21c4e5904
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841330"
---
# <a name="tablesort-clear"></a><span data-ttu-id="99ed1-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="99ed1-104">TableSort: clear</span></span>

> <span data-ttu-id="99ed1-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99ed1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99ed1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99ed1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99ed1-p103">Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="99ed1-p103">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="99ed1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99ed1-109">Permissions</span></span>
<span data-ttu-id="99ed1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99ed1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99ed1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99ed1-112">Permission type</span></span>      | <span data-ttu-id="99ed1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99ed1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99ed1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99ed1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="99ed1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99ed1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99ed1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99ed1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99ed1-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99ed1-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="99ed1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99ed1-118">Application</span></span> | <span data-ttu-id="99ed1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99ed1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99ed1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99ed1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="99ed1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99ed1-121">Request headers</span></span>
| <span data-ttu-id="99ed1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="99ed1-122">Name</span></span>       | <span data-ttu-id="99ed1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="99ed1-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="99ed1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99ed1-124">Authorization</span></span>  | <span data-ttu-id="99ed1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99ed1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="99ed1-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="99ed1-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="99ed1-p106">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="99ed1-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="99ed1-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99ed1-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="99ed1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="99ed1-131">Response</span></span>

<span data-ttu-id="99ed1-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="99ed1-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99ed1-134">Пример</span><span class="sxs-lookup"><span data-stu-id="99ed1-134">Example</span></span>
<span data-ttu-id="99ed1-135">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="99ed1-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99ed1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="99ed1-136">Request</span></span>
<span data-ttu-id="99ed1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99ed1-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="99ed1-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="99ed1-138">Response</span></span>
<span data-ttu-id="99ed1-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="99ed1-139">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
