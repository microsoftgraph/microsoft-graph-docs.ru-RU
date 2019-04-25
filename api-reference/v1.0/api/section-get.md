---
title: Получение раздела
description: Получение свойств и связей объекта Оненотесектион.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d491e0936096296c731e2ebbbc1d6d44dccdef38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521049"
---
# <a name="get-section"></a><span data-ttu-id="c2217-103">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="c2217-103">Get section</span></span>

<span data-ttu-id="c2217-104">Получение свойств и связей объекта [оненотесектион](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="c2217-104">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2217-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2217-105">Permissions</span></span>
<span data-ttu-id="c2217-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2217-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2217-108">Permission type</span></span>      | <span data-ttu-id="c2217-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2217-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2217-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2217-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2217-111">Notes. Create, Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c2217-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2217-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2217-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2217-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2217-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c2217-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2217-114">Application</span></span> | <span data-ttu-id="c2217-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2217-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2217-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2217-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2217-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2217-117">Optional query parameters</span></span>
<span data-ttu-id="c2217-118">Этот метод поддерживает `select` `expand` [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c2217-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c2217-119">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="c2217-119">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="c2217-120">Допустимые `expand` значения для разделов `parentNotebook` — `parentSectionGroup`и.</span><span class="sxs-lookup"><span data-stu-id="c2217-120">Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2217-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2217-121">Request headers</span></span>
| <span data-ttu-id="c2217-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c2217-122">Name</span></span>       | <span data-ttu-id="c2217-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c2217-123">Type</span></span> | <span data-ttu-id="c2217-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c2217-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c2217-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2217-125">Authorization</span></span>  | <span data-ttu-id="c2217-126">string</span><span class="sxs-lookup"><span data-stu-id="c2217-126">string</span></span>  | <span data-ttu-id="c2217-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2217-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2217-129">Accept</span><span class="sxs-lookup"><span data-stu-id="c2217-129">Accept</span></span> | <span data-ttu-id="c2217-130">string</span><span class="sxs-lookup"><span data-stu-id="c2217-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c2217-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2217-131">Request body</span></span>
<span data-ttu-id="c2217-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2217-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2217-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2217-133">Response</span></span>

<span data-ttu-id="c2217-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [оненотесектион](../resources/section.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2217-134">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2217-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c2217-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2217-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2217-136">Request</span></span>
<span data-ttu-id="c2217-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2217-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="c2217-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2217-138">Response</span></span>
<span data-ttu-id="c2217-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2217-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
