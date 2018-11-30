---
title: Перечисление записных книжек
description: Получение списка объектов notebook.
ms.openlocfilehash: 0f9bf502973be0d178db70e42f25a0716263e323
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077055"
---
# <a name="list-notebooks"></a><span data-ttu-id="c99f9-103">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="c99f9-103">List notebooks</span></span>

> <span data-ttu-id="c99f9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c99f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c99f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c99f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c99f9-106">Получение списка объектов [notebook](../resources/notebook.md).</span><span class="sxs-lookup"><span data-stu-id="c99f9-106">Retrieve a list of [notebook](../resources/notebook.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c99f9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c99f9-107">Permissions</span></span>
<span data-ttu-id="c99f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c99f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c99f9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c99f9-110">Permission type</span></span>      | <span data-ttu-id="c99f9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c99f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c99f9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c99f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c99f9-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c99f9-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c99f9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c99f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c99f9-115">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c99f9-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c99f9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c99f9-116">Application</span></span> | <span data-ttu-id="c99f9-117">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c99f9-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c99f9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c99f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks
GET /users/{id | userPrincipalName}/onenote/notebooks
GET /groups/{id}/onenote/notebooks
GET /sites/{id}/onenote/notebooks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c99f9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c99f9-119">Optional query parameters</span></span>
<span data-ttu-id="c99f9-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c99f9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c99f9-121">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c99f9-121">The default sort order is `name asc`.</span></span> 

<span data-ttu-id="c99f9-122">Допустимые значения `expand` для записных книжек: `sections` и `sectionGroups`.</span><span class="sxs-lookup"><span data-stu-id="c99f9-122">Valid `expand` values for notebooks are `sections` and `sectionGroups`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c99f9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c99f9-123">Request headers</span></span>
| <span data-ttu-id="c99f9-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c99f9-124">Name</span></span>       | <span data-ttu-id="c99f9-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c99f9-125">Type</span></span> | <span data-ttu-id="c99f9-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c99f9-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c99f9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c99f9-127">Authorization</span></span>  | <span data-ttu-id="c99f9-128">string</span><span class="sxs-lookup"><span data-stu-id="c99f9-128">string</span></span>  | <span data-ttu-id="c99f9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c99f9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c99f9-131">Accept</span><span class="sxs-lookup"><span data-stu-id="c99f9-131">Accept</span></span> | <span data-ttu-id="c99f9-132">строка</span><span class="sxs-lookup"><span data-stu-id="c99f9-132">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c99f9-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c99f9-133">Request body</span></span>
<span data-ttu-id="c99f9-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c99f9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c99f9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c99f9-135">Response</span></span>

<span data-ttu-id="c99f9-136">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [notebook](../resources/notebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c99f9-136">If successful, this method returns a `200 OK` response code and collection of [notebook](../resources/notebook.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c99f9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="c99f9-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c99f9-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="c99f9-138">Request</span></span>
<span data-ttu-id="c99f9-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c99f9-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_notebooks"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks
```
##### <a name="response"></a><span data-ttu-id="c99f9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c99f9-140">Response</span></span>
<span data-ttu-id="c99f9-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c99f9-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79",
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