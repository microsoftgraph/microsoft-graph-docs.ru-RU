---
title: Получение записной книжки
description: Получение свойств и связей объекта notebook.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: cae976cb7008dcf5802654cb7d8bf379b58c4e4b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839328"
---
# <a name="get-notebook"></a><span data-ttu-id="dbeb8-103">Получение записной книжки</span><span class="sxs-lookup"><span data-stu-id="dbeb8-103">Get notebook</span></span>

<span data-ttu-id="dbeb8-104">Получение свойств и связей объекта [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="dbeb8-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dbeb8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dbeb8-105">Permissions</span></span>
<span data-ttu-id="dbeb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbeb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbeb8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbeb8-108">Permission type</span></span>      | <span data-ttu-id="dbeb8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbeb8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dbeb8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbeb8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dbeb8-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbeb8-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="dbeb8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbeb8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dbeb8-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dbeb8-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="dbeb8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbeb8-114">Application</span></span> | <span data-ttu-id="dbeb8-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbeb8-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dbeb8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbeb8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dbeb8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dbeb8-117">Optional query parameters</span></span>
<span data-ttu-id="dbeb8-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` и `expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dbeb8-118">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="dbeb8-119">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="dbeb8-119">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbeb8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dbeb8-120">Request headers</span></span>
| <span data-ttu-id="dbeb8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dbeb8-121">Name</span></span>       | <span data-ttu-id="dbeb8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="dbeb8-122">Type</span></span> | <span data-ttu-id="dbeb8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dbeb8-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dbeb8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbeb8-124">Authorization</span></span>  | <span data-ttu-id="dbeb8-125">string</span><span class="sxs-lookup"><span data-stu-id="dbeb8-125">string</span></span>  | <span data-ttu-id="dbeb8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbeb8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dbeb8-128">Accept</span><span class="sxs-lookup"><span data-stu-id="dbeb8-128">Accept</span></span> | <span data-ttu-id="dbeb8-129">строка</span><span class="sxs-lookup"><span data-stu-id="dbeb8-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="dbeb8-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dbeb8-130">Request body</span></span>
<span data-ttu-id="dbeb8-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dbeb8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbeb8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbeb8-132">Response</span></span>

<span data-ttu-id="dbeb8-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dbeb8-133">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dbeb8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="dbeb8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dbeb8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbeb8-135">Request</span></span>
<span data-ttu-id="dbeb8-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbeb8-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="dbeb8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbeb8-137">Response</span></span>
<span data-ttu-id="dbeb8-p103">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbeb8-p103">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 284

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get notebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
