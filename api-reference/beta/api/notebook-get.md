---
title: Получение записной книжки
description: Получение свойств и связей объекта notebook.
ms.openlocfilehash: 9dd264dd2498e0c775629b9e178b7660426a8d69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081694"
---
# <a name="get-notebook"></a><span data-ttu-id="37eff-103">Получение записной книжки</span><span class="sxs-lookup"><span data-stu-id="37eff-103">Get notebook</span></span>

> <span data-ttu-id="37eff-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37eff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37eff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37eff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37eff-106">Получение свойств и связей объекта [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="37eff-106">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="37eff-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37eff-107">Permissions</span></span>
<span data-ttu-id="37eff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37eff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37eff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37eff-110">Permission type</span></span>      | <span data-ttu-id="37eff-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37eff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37eff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37eff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="37eff-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37eff-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="37eff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37eff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37eff-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37eff-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="37eff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37eff-116">Application</span></span> | <span data-ttu-id="37eff-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37eff-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37eff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37eff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}
GET /groups/{id}/onenote/notebooks/{id}
GET /sites/{id}/onenote/notebooks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="37eff-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37eff-119">Optional query parameters</span></span>
<span data-ttu-id="37eff-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `select` и `expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="37eff-120">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="37eff-121">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="37eff-121">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37eff-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37eff-122">Request headers</span></span>
| <span data-ttu-id="37eff-123">Имя</span><span class="sxs-lookup"><span data-stu-id="37eff-123">Name</span></span>       | <span data-ttu-id="37eff-124">Тип</span><span class="sxs-lookup"><span data-stu-id="37eff-124">Type</span></span> | <span data-ttu-id="37eff-125">Описание</span><span class="sxs-lookup"><span data-stu-id="37eff-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="37eff-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="37eff-126">Authorization</span></span>  | <span data-ttu-id="37eff-127">string</span><span class="sxs-lookup"><span data-stu-id="37eff-127">string</span></span>  | <span data-ttu-id="37eff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37eff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="37eff-130">Accept</span><span class="sxs-lookup"><span data-stu-id="37eff-130">Accept</span></span> | <span data-ttu-id="37eff-131">строка</span><span class="sxs-lookup"><span data-stu-id="37eff-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="37eff-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37eff-132">Request body</span></span>
<span data-ttu-id="37eff-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37eff-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37eff-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="37eff-134">Response</span></span>

<span data-ttu-id="37eff-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="37eff-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37eff-136">Пример</span><span class="sxs-lookup"><span data-stu-id="37eff-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37eff-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="37eff-137">Request</span></span>
<span data-ttu-id="37eff-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37eff-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebook"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}
```
##### <a name="response"></a><span data-ttu-id="37eff-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="37eff-139">Response</span></span>
<span data-ttu-id="37eff-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37eff-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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
