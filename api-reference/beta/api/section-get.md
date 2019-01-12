---
title: Получение раздела
description: Получение свойств и связей объекта section.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ce475e0bdd8b5557eb2b6c457c6736ac635eb0be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953401"
---
# <a name="get-section"></a><span data-ttu-id="83ba0-103">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="83ba0-103">Get section</span></span>

> <span data-ttu-id="83ba0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="83ba0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83ba0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83ba0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83ba0-106">Получение свойств и связей объекта [section](../resources/section.md).</span><span class="sxs-lookup"><span data-stu-id="83ba0-106">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="83ba0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83ba0-107">Permissions</span></span>
<span data-ttu-id="83ba0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83ba0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83ba0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83ba0-110">Permission type</span></span>      | <span data-ttu-id="83ba0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83ba0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83ba0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83ba0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="83ba0-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83ba0-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="83ba0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83ba0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83ba0-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83ba0-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="83ba0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83ba0-116">Application</span></span> | <span data-ttu-id="83ba0-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83ba0-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83ba0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83ba0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83ba0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="83ba0-119">Optional query parameters</span></span>
<span data-ttu-id="83ba0-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` и `expand` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="83ba0-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="83ba0-p103">Запрос по умолчанию разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="83ba0-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83ba0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83ba0-123">Request headers</span></span>
| <span data-ttu-id="83ba0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="83ba0-124">Name</span></span>       | <span data-ttu-id="83ba0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="83ba0-125">Type</span></span> | <span data-ttu-id="83ba0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="83ba0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="83ba0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="83ba0-127">Authorization</span></span>  | <span data-ttu-id="83ba0-128">string</span><span class="sxs-lookup"><span data-stu-id="83ba0-128">string</span></span>  | <span data-ttu-id="83ba0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83ba0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83ba0-131">Accept</span><span class="sxs-lookup"><span data-stu-id="83ba0-131">Accept</span></span> | <span data-ttu-id="83ba0-132">строка</span><span class="sxs-lookup"><span data-stu-id="83ba0-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="83ba0-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83ba0-133">Request body</span></span>
<span data-ttu-id="83ba0-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83ba0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83ba0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="83ba0-135">Response</span></span>

<span data-ttu-id="83ba0-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [section](../resources/section.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="83ba0-136">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83ba0-137">Пример</span><span class="sxs-lookup"><span data-stu-id="83ba0-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83ba0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="83ba0-138">Request</span></span>
<span data-ttu-id="83ba0-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83ba0-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="83ba0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="83ba0-140">Response</span></span>
<span data-ttu-id="83ba0-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83ba0-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
