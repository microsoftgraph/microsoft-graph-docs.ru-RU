---
title: Перечисление разделов
description: Получение списка объектов section из указанной записной книжки.
author: Jewan-microsoft
ms.openlocfilehash: ab1f531e687f3b17c18b2b61067eee5e9283acb7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332398"
---
# <a name="list-sections"></a><span data-ttu-id="fb748-103">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="fb748-103">List sections</span></span>

> <span data-ttu-id="fb748-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb748-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb748-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb748-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb748-106">Получение списка объектов [section](../resources/section.md) из указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="fb748-106">Retrieve a list of [section](../resources/section.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="fb748-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb748-107">Permissions</span></span>
<span data-ttu-id="fb748-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb748-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb748-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb748-110">Permission type</span></span>      | <span data-ttu-id="fb748-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb748-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb748-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb748-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fb748-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb748-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb748-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb748-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb748-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb748-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="fb748-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb748-116">Application</span></span> | <span data-ttu-id="fb748-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb748-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb748-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb748-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb748-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb748-119">Optional query parameters</span></span>
<span data-ttu-id="fb748-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fb748-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="fb748-121">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="fb748-121">The default sort order is `name asc`.</span></span>

<span data-ttu-id="fb748-p103">Запрос, используемый по умолчанию, разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="fb748-p103">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="fb748-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb748-124">Request headers</span></span>
| <span data-ttu-id="fb748-125">Имя</span><span class="sxs-lookup"><span data-stu-id="fb748-125">Name</span></span>       | <span data-ttu-id="fb748-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fb748-126">Type</span></span> | <span data-ttu-id="fb748-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fb748-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fb748-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb748-128">Authorization</span></span>  | <span data-ttu-id="fb748-129">string</span><span class="sxs-lookup"><span data-stu-id="fb748-129">string</span></span>  | <span data-ttu-id="fb748-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb748-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fb748-132">Accept</span><span class="sxs-lookup"><span data-stu-id="fb748-132">Accept</span></span> | <span data-ttu-id="fb748-133">строка</span><span class="sxs-lookup"><span data-stu-id="fb748-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="fb748-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb748-134">Request body</span></span>
<span data-ttu-id="fb748-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb748-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb748-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb748-136">Response</span></span>

<span data-ttu-id="fb748-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [section](../resources/section.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fb748-137">If successful, this method returns a `200 OK` response code and a collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb748-138">Пример</span><span class="sxs-lookup"><span data-stu-id="fb748-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb748-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb748-139">Request</span></span>
<span data-ttu-id="fb748-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb748-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="fb748-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb748-141">Response</span></span>
<span data-ttu-id="fb748-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb748-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
