---
title: 'Filter: clear'
description: Сбрасывает фильтр для определенного столбца.
localization_priority: Normal
ms.openlocfilehash: 9dd13991572d28e61dafce3049698117729161fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838187"
---
# <a name="filter-clear"></a><span data-ttu-id="1657b-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="1657b-103">Filter: clear</span></span>

> <span data-ttu-id="1657b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1657b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1657b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1657b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1657b-106">Сброс фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="1657b-106">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="1657b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1657b-107">Permissions</span></span>
<span data-ttu-id="1657b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1657b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1657b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1657b-110">Permission type</span></span>      | <span data-ttu-id="1657b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1657b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1657b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1657b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1657b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1657b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1657b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1657b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1657b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1657b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1657b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1657b-116">Application</span></span> | <span data-ttu-id="1657b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1657b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1657b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1657b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="1657b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1657b-119">Request headers</span></span>
| <span data-ttu-id="1657b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1657b-120">Name</span></span>       | <span data-ttu-id="1657b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1657b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1657b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1657b-122">Authorization</span></span>  | <span data-ttu-id="1657b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1657b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1657b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1657b-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1657b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1657b-126">Response</span></span>

<span data-ttu-id="1657b-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1657b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1657b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1657b-129">Example</span></span>
<span data-ttu-id="1657b-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1657b-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1657b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1657b-131">Request</span></span>
<span data-ttu-id="1657b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1657b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="1657b-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="1657b-133">Response</span></span>
<span data-ttu-id="1657b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1657b-134">Here is an example of the response.</span></span> 
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
