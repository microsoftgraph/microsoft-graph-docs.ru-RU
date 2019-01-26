---
title: Перечисление sectionGroups
description: Получение списка объектов sectionGroup.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 80c2391e1c6cf71614314310bb67032734a519b2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576964"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="49d8e-103">Перечисление sectionGroups</span><span class="sxs-lookup"><span data-stu-id="49d8e-103">List sectionGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49d8e-104">Получение списка объектов [sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="49d8e-104">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="49d8e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49d8e-105">Permissions</span></span>
<span data-ttu-id="49d8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49d8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49d8e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49d8e-108">Permission type</span></span>      | <span data-ttu-id="49d8e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49d8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49d8e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49d8e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49d8e-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49d8e-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="49d8e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49d8e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49d8e-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49d8e-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="49d8e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49d8e-114">Application</span></span> | <span data-ttu-id="49d8e-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49d8e-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49d8e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49d8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49d8e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49d8e-117">Optional query parameters</span></span>
<span data-ttu-id="49d8e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="49d8e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="49d8e-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="49d8e-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="49d8e-p102">Запрос, используемый по умолчанию, разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для групп разделов: `sections`, `sectionGroups`, `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="49d8e-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49d8e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49d8e-122">Request headers</span></span>
| <span data-ttu-id="49d8e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="49d8e-123">Name</span></span>       | <span data-ttu-id="49d8e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="49d8e-124">Type</span></span> | <span data-ttu-id="49d8e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="49d8e-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="49d8e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="49d8e-126">Authorization</span></span>  | <span data-ttu-id="49d8e-127">string</span><span class="sxs-lookup"><span data-stu-id="49d8e-127">string</span></span>  | <span data-ttu-id="49d8e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49d8e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49d8e-130">Accept</span><span class="sxs-lookup"><span data-stu-id="49d8e-130">Accept</span></span> | <span data-ttu-id="49d8e-131">строка</span><span class="sxs-lookup"><span data-stu-id="49d8e-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="49d8e-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49d8e-132">Request body</span></span>
<span data-ttu-id="49d8e-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49d8e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49d8e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="49d8e-134">Response</span></span>

<span data-ttu-id="49d8e-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="49d8e-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49d8e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="49d8e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49d8e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="49d8e-137">Request</span></span>
<span data-ttu-id="49d8e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49d8e-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="49d8e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="49d8e-139">Response</span></span>
<span data-ttu-id="49d8e-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49d8e-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
    {
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "displayName": "name-value",
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onenote-list-sectiongroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
