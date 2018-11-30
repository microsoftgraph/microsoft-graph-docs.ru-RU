---
title: 'Filter: clear'
description: Сброс фильтра для определенного столбца.
ms.openlocfilehash: ae71723ed3ca9074bb7a71ea131fd7103f3714af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076582"
---
# <a name="filter-clear"></a><span data-ttu-id="405af-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="405af-103">Filter: clear</span></span>

> <span data-ttu-id="405af-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="405af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="405af-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="405af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="405af-106">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="405af-106">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="405af-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="405af-107">Permissions</span></span>
<span data-ttu-id="405af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="405af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="405af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="405af-110">Permission type</span></span>      | <span data-ttu-id="405af-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="405af-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="405af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="405af-112">Delegated (work or school account)</span></span> | <span data-ttu-id="405af-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="405af-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="405af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="405af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="405af-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="405af-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="405af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="405af-116">Application</span></span> | <span data-ttu-id="405af-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="405af-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="405af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="405af-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="405af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="405af-119">Request headers</span></span>
| <span data-ttu-id="405af-120">Имя</span><span class="sxs-lookup"><span data-stu-id="405af-120">Name</span></span>       | <span data-ttu-id="405af-121">Описание</span><span class="sxs-lookup"><span data-stu-id="405af-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="405af-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="405af-122">Authorization</span></span>  | <span data-ttu-id="405af-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="405af-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="405af-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="405af-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="405af-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="405af-126">Response</span></span>

<span data-ttu-id="405af-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="405af-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="405af-129">Пример</span><span class="sxs-lookup"><span data-stu-id="405af-129">Example</span></span>
<span data-ttu-id="405af-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="405af-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="405af-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="405af-131">Request</span></span>
<span data-ttu-id="405af-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="405af-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="405af-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="405af-133">Response</span></span>
<span data-ttu-id="405af-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="405af-134">Here is an example of the response.</span></span> 
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
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->