---
title: Получение раздела
description: Получение свойств и связей объекта section.
ms.openlocfilehash: e4e46a220e02b5fe98e18a1f62125c7697efe052
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075081"
---
# <a name="get-section"></a><span data-ttu-id="6bd72-103">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="6bd72-103">Get section</span></span>

> <span data-ttu-id="6bd72-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6bd72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bd72-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bd72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6bd72-106">Получение свойств и связей объекта [section](../resources/section.md).</span><span class="sxs-lookup"><span data-stu-id="6bd72-106">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6bd72-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bd72-107">Permissions</span></span>
<span data-ttu-id="6bd72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bd72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bd72-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bd72-110">Permission type</span></span>      | <span data-ttu-id="6bd72-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bd72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bd72-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bd72-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6bd72-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bd72-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6bd72-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bd72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bd72-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6bd72-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6bd72-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bd72-116">Application</span></span> | <span data-ttu-id="6bd72-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bd72-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bd72-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bd72-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6bd72-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6bd72-119">Optional query parameters</span></span>
<span data-ttu-id="6bd72-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` и `expand` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6bd72-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="6bd72-p103">Запрос по умолчанию разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="6bd72-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bd72-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bd72-123">Request headers</span></span>
| <span data-ttu-id="6bd72-124">Имя</span><span class="sxs-lookup"><span data-stu-id="6bd72-124">Name</span></span>       | <span data-ttu-id="6bd72-125">Тип</span><span class="sxs-lookup"><span data-stu-id="6bd72-125">Type</span></span> | <span data-ttu-id="6bd72-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6bd72-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6bd72-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bd72-127">Authorization</span></span>  | <span data-ttu-id="6bd72-128">string</span><span class="sxs-lookup"><span data-stu-id="6bd72-128">string</span></span>  | <span data-ttu-id="6bd72-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bd72-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6bd72-131">Accept</span><span class="sxs-lookup"><span data-stu-id="6bd72-131">Accept</span></span> | <span data-ttu-id="6bd72-132">строка</span><span class="sxs-lookup"><span data-stu-id="6bd72-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6bd72-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6bd72-133">Request body</span></span>
<span data-ttu-id="6bd72-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6bd72-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bd72-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bd72-135">Response</span></span>

<span data-ttu-id="6bd72-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [section](../resources/section.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6bd72-136">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6bd72-137">Пример</span><span class="sxs-lookup"><span data-stu-id="6bd72-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6bd72-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bd72-138">Request</span></span>
<span data-ttu-id="6bd72-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bd72-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="6bd72-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bd72-140">Response</span></span>
<span data-ttu-id="6bd72-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6bd72-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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