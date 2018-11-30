---
title: Перечисление разделов
description: Получение списка объектов onenoteSection из указанного раздела группы.
ms.openlocfilehash: 0298293f1f82cd61d376e195360b79d4a96d5344
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026212"
---
# <a name="list-sections"></a><span data-ttu-id="42653-103">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="42653-103">List sections</span></span>

<span data-ttu-id="42653-104">Получение списка объектов [onenoteSection](../resources/section.md) из указанного раздела группы.</span><span class="sxs-lookup"><span data-stu-id="42653-104">Retrieve a list of [onenoteSection](../resources/section.md) objects from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="42653-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42653-105">Permissions</span></span>
<span data-ttu-id="42653-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42653-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42653-108">Permission type</span></span>      | <span data-ttu-id="42653-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42653-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42653-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42653-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42653-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42653-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="42653-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42653-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42653-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42653-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="42653-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42653-114">Application</span></span> | <span data-ttu-id="42653-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42653-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="42653-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42653-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42653-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42653-117">Optional query parameters</span></span>
<span data-ttu-id="42653-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="42653-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="42653-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="42653-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="42653-p102">Запрос, используемый по умолчанию, разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="42653-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="42653-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42653-122">Request headers</span></span>
| <span data-ttu-id="42653-123">Имя</span><span class="sxs-lookup"><span data-stu-id="42653-123">Name</span></span>       | <span data-ttu-id="42653-124">Тип</span><span class="sxs-lookup"><span data-stu-id="42653-124">Type</span></span> | <span data-ttu-id="42653-125">Описание</span><span class="sxs-lookup"><span data-stu-id="42653-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="42653-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="42653-126">Authorization</span></span>  | <span data-ttu-id="42653-127">string</span><span class="sxs-lookup"><span data-stu-id="42653-127">string</span></span>  | <span data-ttu-id="42653-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42653-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="42653-130">Accept</span><span class="sxs-lookup"><span data-stu-id="42653-130">Accept</span></span> | <span data-ttu-id="42653-131">строка</span><span class="sxs-lookup"><span data-stu-id="42653-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="42653-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42653-132">Request body</span></span>
<span data-ttu-id="42653-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42653-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42653-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="42653-134">Response</span></span>

<span data-ttu-id="42653-135">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [onenoteSection](../resources/section.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="42653-135">If successful, this method returns a `200 OK` response code and a collection of [onenoteSection](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42653-136">Пример</span><span class="sxs-lookup"><span data-stu-id="42653-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42653-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="42653-137">Request</span></span>
<span data-ttu-id="42653-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42653-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="42653-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="42653-139">Response</span></span>
<span data-ttu-id="42653-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42653-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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