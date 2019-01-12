---
title: Перечисление разделов
description: Получение списка объектов section из указанной группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 66ffe610df5479eac78a943b1eefac0a41ecd37e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953359"
---
# <a name="list-sections"></a><span data-ttu-id="a4620-103">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="a4620-103">List sections</span></span>

> <span data-ttu-id="a4620-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a4620-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4620-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4620-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4620-106">Получение списка объектов [section](../resources/section.md) из указанной группы разделов.</span><span class="sxs-lookup"><span data-stu-id="a4620-106">Retrieve a list of [section](../resources/section.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="a4620-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4620-107">Permissions</span></span>
<span data-ttu-id="a4620-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4620-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4620-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4620-110">Permission type</span></span>      | <span data-ttu-id="a4620-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4620-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4620-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4620-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a4620-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4620-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a4620-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4620-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4620-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4620-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a4620-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4620-116">Application</span></span> | <span data-ttu-id="a4620-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4620-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4620-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4620-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a4620-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4620-119">Optional query parameters</span></span>
<span data-ttu-id="a4620-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a4620-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a4620-121">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="a4620-121">The default sort order is `name asc`.</span></span>

<span data-ttu-id="a4620-p103">Запрос, используемый по умолчанию, разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="a4620-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="a4620-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4620-124">Request headers</span></span>
| <span data-ttu-id="a4620-125">Имя</span><span class="sxs-lookup"><span data-stu-id="a4620-125">Name</span></span>       | <span data-ttu-id="a4620-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a4620-126">Type</span></span> | <span data-ttu-id="a4620-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a4620-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a4620-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4620-128">Authorization</span></span>  | <span data-ttu-id="a4620-129">string</span><span class="sxs-lookup"><span data-stu-id="a4620-129">string</span></span>  | <span data-ttu-id="a4620-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4620-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4620-132">Accept</span><span class="sxs-lookup"><span data-stu-id="a4620-132">Accept</span></span> | <span data-ttu-id="a4620-133">строка</span><span class="sxs-lookup"><span data-stu-id="a4620-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a4620-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4620-134">Request body</span></span>
<span data-ttu-id="a4620-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4620-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4620-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4620-136">Response</span></span>

<span data-ttu-id="a4620-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [section](../resources/section.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a4620-137">If successful, this method returns a `200 OK` response code and a collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a4620-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a4620-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4620-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4620-139">Request</span></span>
<span data-ttu-id="a4620-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4620-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="a4620-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4620-141">Response</span></span>
<span data-ttu-id="a4620-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4620-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
