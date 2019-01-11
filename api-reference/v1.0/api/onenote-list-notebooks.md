---
title: Перечисление записных книжек
description: Получение списка объектов notebook.
author: Jewan-microsoft
localization_priority: Priority
ms.openlocfilehash: 5a6ae25ab048e0f0e9b25144957add5bbf85d615
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810152"
---
# <a name="list-notebooks"></a><span data-ttu-id="8075d-103">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="8075d-103">List notebooks</span></span>

<span data-ttu-id="8075d-104">Получение списка объектов [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="8075d-104">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8075d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8075d-105">Permissions</span></span>
<span data-ttu-id="8075d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8075d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8075d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8075d-108">Permission type</span></span>      | <span data-ttu-id="8075d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8075d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8075d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8075d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8075d-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8075d-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="8075d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8075d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8075d-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8075d-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="8075d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8075d-114">Application</span></span> | <span data-ttu-id="8075d-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8075d-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8075d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8075d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8075d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8075d-117">Optional query parameters</span></span>
<span data-ttu-id="8075d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8075d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8075d-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="8075d-119">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="8075d-120">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="8075d-120">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8075d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8075d-121">Request headers</span></span>
| <span data-ttu-id="8075d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8075d-122">Name</span></span>       | <span data-ttu-id="8075d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8075d-123">Type</span></span> | <span data-ttu-id="8075d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8075d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8075d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8075d-125">Authorization</span></span>  | <span data-ttu-id="8075d-126">string</span><span class="sxs-lookup"><span data-stu-id="8075d-126">string</span></span>  | <span data-ttu-id="8075d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8075d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8075d-129">Accept</span><span class="sxs-lookup"><span data-stu-id="8075d-129">Accept</span></span> | <span data-ttu-id="8075d-130">строка</span><span class="sxs-lookup"><span data-stu-id="8075d-130">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="8075d-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8075d-131">Request body</span></span>
<span data-ttu-id="8075d-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8075d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8075d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8075d-133">Response</span></span>

<span data-ttu-id="8075d-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8075d-134">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8075d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8075d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8075d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8075d-136">Request</span></span>
<span data-ttu-id="8075d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8075d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="8075d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8075d-138">Response</span></span>
<span data-ttu-id="8075d-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8075d-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 369

{
  "value": [
    {
      "isDefault": true,
      "userRole": {
      },
      "isShared": true,
      "sectionsUrl": "sectionsUrl-value",
      "sectionGroupsUrl": "sectionGroupsUrl-value",
      "links": {
        "oneNoteClientUrl": {
          "href": "href-value"
        },
        "oneNoteWebUrl": {
          "href": "href-value"
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
  "description": "List notebooks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
