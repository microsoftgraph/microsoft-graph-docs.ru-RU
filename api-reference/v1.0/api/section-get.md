---
title: Получение раздела
description: Извлечение свойств и связи объекта onenoteSection.
localization_priority: Normal
ms.openlocfilehash: 56a8715ddbc2152dcf131122fded7b4495a8e378
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819980"
---
# <a name="get-section"></a><span data-ttu-id="f6a8d-103">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="f6a8d-103">Get section</span></span>

<span data-ttu-id="f6a8d-104">Извлечение свойств и связи объекта [onenoteSection](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="f6a8d-104">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6a8d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6a8d-105">Permissions</span></span>
<span data-ttu-id="f6a8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6a8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6a8d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6a8d-108">Permission type</span></span>      | <span data-ttu-id="f6a8d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6a8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6a8d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6a8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6a8d-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6a8d-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6a8d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6a8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6a8d-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6a8d-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="f6a8d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6a8d-114">Application</span></span> | <span data-ttu-id="f6a8d-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6a8d-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6a8d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6a8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6a8d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6a8d-117">Optional query parameters</span></span>
<span data-ttu-id="f6a8d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` и `expand` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6a8d-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f6a8d-p102">Запрос по умолчанию разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="f6a8d-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6a8d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6a8d-121">Request headers</span></span>
| <span data-ttu-id="f6a8d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f6a8d-122">Name</span></span>       | <span data-ttu-id="f6a8d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f6a8d-123">Type</span></span> | <span data-ttu-id="f6a8d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f6a8d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6a8d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6a8d-125">Authorization</span></span>  | <span data-ttu-id="f6a8d-126">string</span><span class="sxs-lookup"><span data-stu-id="f6a8d-126">string</span></span>  | <span data-ttu-id="f6a8d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6a8d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6a8d-129">Accept</span><span class="sxs-lookup"><span data-stu-id="f6a8d-129">Accept</span></span> | <span data-ttu-id="f6a8d-130">строка</span><span class="sxs-lookup"><span data-stu-id="f6a8d-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f6a8d-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6a8d-131">Request body</span></span>
<span data-ttu-id="f6a8d-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6a8d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6a8d-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6a8d-133">Response</span></span>

<span data-ttu-id="f6a8d-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [onenoteSection](../resources/section.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f6a8d-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6a8d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f6a8d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6a8d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6a8d-136">Request</span></span>
<span data-ttu-id="f6a8d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6a8d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="f6a8d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6a8d-138">Response</span></span>
<span data-ttu-id="f6a8d-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6a8d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
