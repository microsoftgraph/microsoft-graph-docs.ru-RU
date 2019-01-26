---
title: Получение объекта sectionGroup
description: Получение свойств и связей объекта sectionGroup.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7b0f0b0ec19c64a6e703ce41d024b3112c354da7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575690"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="e297f-103">Получение объекта sectionGroup</span><span class="sxs-lookup"><span data-stu-id="e297f-103">Get sectionGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e297f-104">Получение свойств и связей объекта [sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="e297f-104">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e297f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e297f-105">Permissions</span></span>
<span data-ttu-id="e297f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e297f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e297f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e297f-108">Permission type</span></span>      | <span data-ttu-id="e297f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e297f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e297f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e297f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e297f-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e297f-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e297f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e297f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e297f-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e297f-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e297f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e297f-114">Application</span></span> | <span data-ttu-id="e297f-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e297f-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e297f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e297f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e297f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e297f-117">Optional query parameters</span></span>
<span data-ttu-id="e297f-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e297f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="e297f-p102">Запрос по умолчанию разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `name` и `self`. Допустимые значения `expand` для групп разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="e297f-p102">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e297f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e297f-121">Request headers</span></span>
| <span data-ttu-id="e297f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e297f-122">Name</span></span>       | <span data-ttu-id="e297f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e297f-123">Type</span></span> | <span data-ttu-id="e297f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e297f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e297f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e297f-125">Authorization</span></span>  | <span data-ttu-id="e297f-126">string</span><span class="sxs-lookup"><span data-stu-id="e297f-126">string</span></span>  | <span data-ttu-id="e297f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e297f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e297f-129">Accept</span><span class="sxs-lookup"><span data-stu-id="e297f-129">Accept</span></span> | <span data-ttu-id="e297f-130">строка</span><span class="sxs-lookup"><span data-stu-id="e297f-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e297f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e297f-131">Request body</span></span>
<span data-ttu-id="e297f-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e297f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e297f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e297f-133">Response</span></span>

<span data-ttu-id="e297f-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e297f-134">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e297f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e297f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e297f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e297f-136">Request</span></span>
<span data-ttu-id="e297f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e297f-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="e297f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e297f-138">Response</span></span>
<span data-ttu-id="e297f-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e297f-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/sectiongroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
