---
title: Список sectionGroups
description: Получение списка объектов sectionGroup.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 86e1cf3ee6963549344b9932597f3ab075149697
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333063"
---
# <a name="list-sectiongroups"></a><span data-ttu-id="27a2c-103">Список sectionGroups</span><span class="sxs-lookup"><span data-stu-id="27a2c-103">List sectionGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27a2c-104">Получение списка объектов [sectionGroup](../resources/sectiongroup.md) .</span><span class="sxs-lookup"><span data-stu-id="27a2c-104">Retrieve a list of [sectionGroup](../resources/sectiongroup.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="27a2c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27a2c-105">Permissions</span></span>
<span data-ttu-id="27a2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27a2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27a2c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27a2c-108">Permission type</span></span>      | <span data-ttu-id="27a2c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27a2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27a2c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27a2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27a2c-111">Notes. Create, Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="27a2c-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="27a2c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27a2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27a2c-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27a2c-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="27a2c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27a2c-114">Application</span></span> | <span data-ttu-id="27a2c-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a2c-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27a2c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27a2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups
GET /groups/{id}/onenote/sectionGroups
GET /sites/{id}/onenote/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27a2c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="27a2c-117">Optional query parameters</span></span>
<span data-ttu-id="27a2c-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="27a2c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="27a2c-119">По умолчанию используется `name asc`порядок сортировки.</span><span class="sxs-lookup"><span data-stu-id="27a2c-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="27a2c-120">Запрос по умолчанию `parentNotebook` разворачивает и выбирает `id`свойства `displayName`, и `self` .</span><span class="sxs-lookup"><span data-stu-id="27a2c-120">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties.</span></span> <span data-ttu-id="27a2c-121">Допустимые `expand` значения для групп разделов `sections`: `sectionGroups`, `parentNotebook`, и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="27a2c-121">Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27a2c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27a2c-122">Request headers</span></span>
| <span data-ttu-id="27a2c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="27a2c-123">Name</span></span>       | <span data-ttu-id="27a2c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="27a2c-124">Type</span></span> | <span data-ttu-id="27a2c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="27a2c-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="27a2c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="27a2c-126">Authorization</span></span>  | <span data-ttu-id="27a2c-127">string</span><span class="sxs-lookup"><span data-stu-id="27a2c-127">string</span></span>  | <span data-ttu-id="27a2c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27a2c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27a2c-130">Accept</span><span class="sxs-lookup"><span data-stu-id="27a2c-130">Accept</span></span> | <span data-ttu-id="27a2c-131">string</span><span class="sxs-lookup"><span data-stu-id="27a2c-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="27a2c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27a2c-132">Request body</span></span>
<span data-ttu-id="27a2c-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27a2c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27a2c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="27a2c-134">Response</span></span>

<span data-ttu-id="27a2c-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [sectionGroup](../resources/sectiongroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27a2c-135">If successful, this method returns a `200 OK` response code and collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27a2c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="27a2c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27a2c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a2c-137">Request</span></span>
<span data-ttu-id="27a2c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27a2c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="27a2c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a2c-139">Response</span></span>
<span data-ttu-id="27a2c-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27a2c-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
