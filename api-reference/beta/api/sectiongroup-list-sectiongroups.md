---
title: Перечисление sectionGroups
description: Получение списка групп разделов из указанной группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: df313533154862017e0cb2dc96a5a75d83ba27ca
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643484"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="25b24-103">Перечисление sectionGroups</span><span class="sxs-lookup"><span data-stu-id="25b24-103">List sectionGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25b24-104">Получение списка [групп разделов](../resources/sectiongroup.md) из указанной группы разделов.</span><span class="sxs-lookup"><span data-stu-id="25b24-104">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="25b24-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25b24-105">Permissions</span></span>
<span data-ttu-id="25b24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25b24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25b24-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25b24-108">Permission type</span></span>      | <span data-ttu-id="25b24-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25b24-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25b24-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25b24-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25b24-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25b24-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="25b24-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25b24-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25b24-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25b24-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="25b24-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25b24-114">Application</span></span> | <span data-ttu-id="25b24-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25b24-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25b24-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25b24-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
GET /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
GET /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="25b24-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25b24-117">Optional query parameters</span></span>
<span data-ttu-id="25b24-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="25b24-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="25b24-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="25b24-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="25b24-p102">Запрос, используемый по умолчанию, разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для групп разделов: `sections`, `sectionGroups`, `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="25b24-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25b24-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25b24-122">Request headers</span></span>
| <span data-ttu-id="25b24-123">Имя</span><span class="sxs-lookup"><span data-stu-id="25b24-123">Name</span></span>       | <span data-ttu-id="25b24-124">Тип</span><span class="sxs-lookup"><span data-stu-id="25b24-124">Type</span></span> | <span data-ttu-id="25b24-125">Описание</span><span class="sxs-lookup"><span data-stu-id="25b24-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="25b24-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="25b24-126">Authorization</span></span>  | <span data-ttu-id="25b24-127">строка</span><span class="sxs-lookup"><span data-stu-id="25b24-127">string</span></span>  | <span data-ttu-id="25b24-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25b24-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25b24-130">Accept</span><span class="sxs-lookup"><span data-stu-id="25b24-130">Accept</span></span> | <span data-ttu-id="25b24-131">строка</span><span class="sxs-lookup"><span data-stu-id="25b24-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="25b24-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25b24-132">Request body</span></span>
<span data-ttu-id="25b24-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25b24-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25b24-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="25b24-134">Response</span></span>

<span data-ttu-id="25b24-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="25b24-135">If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25b24-136">Пример</span><span class="sxs-lookup"><span data-stu-id="25b24-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25b24-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="25b24-137">Request</span></span>
<span data-ttu-id="25b24-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25b24-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="25b24-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="25b24-139">Response</span></span>
<span data-ttu-id="25b24-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25b24-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup",
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
    "Error: /api-reference/beta/api/sectiongroup-list-sectiongroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
