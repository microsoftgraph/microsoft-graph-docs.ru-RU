---
title: 'Filter: apply'
description: Применяет заданные условия фильтра для определенного столбца.
localization_priority: Normal
ms.openlocfilehash: 3b37344ae3047b54488fa0dd95944c0f34e3bd2b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882903"
---
# <a name="filter-apply"></a><span data-ttu-id="35381-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="35381-103">Filter: apply</span></span>

> <span data-ttu-id="35381-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35381-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35381-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35381-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35381-106">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="35381-106">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="35381-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35381-107">Permissions</span></span>
<span data-ttu-id="35381-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35381-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35381-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35381-110">Permission type</span></span>      | <span data-ttu-id="35381-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35381-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35381-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35381-112">Delegated (work or school account)</span></span> | <span data-ttu-id="35381-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35381-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="35381-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35381-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35381-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35381-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="35381-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35381-116">Application</span></span> | <span data-ttu-id="35381-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35381-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35381-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35381-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="35381-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35381-119">Request headers</span></span>
| <span data-ttu-id="35381-120">Имя</span><span class="sxs-lookup"><span data-stu-id="35381-120">Name</span></span>       | <span data-ttu-id="35381-121">Описание</span><span class="sxs-lookup"><span data-stu-id="35381-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="35381-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35381-122">Authorization</span></span>  | <span data-ttu-id="35381-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35381-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35381-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35381-125">Request body</span></span>
<span data-ttu-id="35381-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="35381-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="35381-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="35381-127">Parameter</span></span>    | <span data-ttu-id="35381-128">Тип</span><span class="sxs-lookup"><span data-stu-id="35381-128">Type</span></span>   |<span data-ttu-id="35381-129">Описание</span><span class="sxs-lookup"><span data-stu-id="35381-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35381-130">criteria</span><span class="sxs-lookup"><span data-stu-id="35381-130">criteria</span></span>|<span data-ttu-id="35381-131">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="35381-131">FilterCriteria</span></span>|<span data-ttu-id="35381-132">Применяемые условия.</span><span class="sxs-lookup"><span data-stu-id="35381-132">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="35381-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="35381-133">Response</span></span>

<span data-ttu-id="35381-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="35381-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35381-136">Пример</span><span class="sxs-lookup"><span data-stu-id="35381-136">Example</span></span>
<span data-ttu-id="35381-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="35381-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="35381-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="35381-138">Request</span></span>
<span data-ttu-id="35381-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35381-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="35381-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="35381-140">Response</span></span>
<span data-ttu-id="35381-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35381-141">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
