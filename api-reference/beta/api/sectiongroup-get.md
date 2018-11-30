---
title: Получение объекта sectionGroup
description: Получение свойств и связей объекта sectionGroup.
ms.openlocfilehash: 12ba258056ae1a317541e01b6747e8de5a97450f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081682"
---
# <a name="get-sectiongroup"></a><span data-ttu-id="b3c67-103">Получение объекта sectionGroup</span><span class="sxs-lookup"><span data-stu-id="b3c67-103">Get sectionGroup</span></span>

> <span data-ttu-id="b3c67-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3c67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3c67-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3c67-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3c67-106">Получение свойств и связей объекта [sectionGroup](../resources/sectiongroup.md).</span><span class="sxs-lookup"><span data-stu-id="b3c67-106">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3c67-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3c67-107">Permissions</span></span>
<span data-ttu-id="b3c67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3c67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3c67-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3c67-110">Permission type</span></span>      | <span data-ttu-id="b3c67-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3c67-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3c67-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3c67-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b3c67-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3c67-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3c67-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3c67-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3c67-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3c67-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b3c67-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3c67-116">Application</span></span> | <span data-ttu-id="b3c67-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3c67-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3c67-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3c67-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3c67-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3c67-119">Optional query parameters</span></span>
<span data-ttu-id="b3c67-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b3c67-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b3c67-p103">Запрос по умолчанию разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `name` и `self`. Допустимые значения `expand` для групп разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="b3c67-p103">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3c67-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3c67-123">Request headers</span></span>
| <span data-ttu-id="b3c67-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b3c67-124">Name</span></span>       | <span data-ttu-id="b3c67-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b3c67-125">Type</span></span> | <span data-ttu-id="b3c67-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b3c67-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b3c67-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3c67-127">Authorization</span></span>  | <span data-ttu-id="b3c67-128">string</span><span class="sxs-lookup"><span data-stu-id="b3c67-128">string</span></span>  | <span data-ttu-id="b3c67-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3c67-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3c67-131">Accept</span><span class="sxs-lookup"><span data-stu-id="b3c67-131">Accept</span></span> | <span data-ttu-id="b3c67-132">строка</span><span class="sxs-lookup"><span data-stu-id="b3c67-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b3c67-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3c67-133">Request body</span></span>
<span data-ttu-id="b3c67-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3c67-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3c67-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3c67-135">Response</span></span>

<span data-ttu-id="b3c67-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [sectionGroup](../resources/sectiongroup.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3c67-136">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3c67-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b3c67-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3c67-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3c67-138">Request</span></span>
<span data-ttu-id="b3c67-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3c67-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="b3c67-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3c67-140">Response</span></span>
<span data-ttu-id="b3c67-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3c67-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectiongroup"
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
<!-- {
  "type": "#page.annotation",
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->