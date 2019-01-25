---
title: Перечисление разделов
description: Получение списка объектов section из указанной записной книжки.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 6f9894b00db6ba7a90613628cd3367b78ce288b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528951"
---
# <a name="list-sections"></a><span data-ttu-id="266d9-103">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="266d9-103">List sections</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="266d9-104">Получение списка объектов [section](../resources/section.md) из указанной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="266d9-104">Retrieve a list of [section](../resources/section.md) objects from the specified notebook.</span></span>
## <a name="permissions"></a><span data-ttu-id="266d9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="266d9-105">Permissions</span></span>
<span data-ttu-id="266d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="266d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="266d9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="266d9-108">Permission type</span></span>      | <span data-ttu-id="266d9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="266d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="266d9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="266d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="266d9-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="266d9-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="266d9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="266d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="266d9-113">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="266d9-113">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="266d9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="266d9-114">Application</span></span> | <span data-ttu-id="266d9-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="266d9-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="266d9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="266d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/{id}/sections
GET /users/{id | userPrincipalName}/onenote/notebooks/{id}/sections
GET /groups/{id}/onenote/notebooks/{id}/sections
GET /sites/{id}/onenote/notebooks/{id}/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="266d9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="266d9-117">Optional query parameters</span></span>
<span data-ttu-id="266d9-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="266d9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="266d9-119">По умолчанию используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="266d9-119">The default sort order is `name asc`.</span></span>

<span data-ttu-id="266d9-p102">Запрос, используемый по умолчанию, разворачивает `parentNotebook` и выбирает соответствующие свойства `id`, `displayName` и `self`. Допустимые значения `expand` для разделов: `parentNotebook` и `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="266d9-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="266d9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="266d9-122">Request headers</span></span>
| <span data-ttu-id="266d9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="266d9-123">Name</span></span>       | <span data-ttu-id="266d9-124">Тип</span><span class="sxs-lookup"><span data-stu-id="266d9-124">Type</span></span> | <span data-ttu-id="266d9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="266d9-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="266d9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="266d9-126">Authorization</span></span>  | <span data-ttu-id="266d9-127">string</span><span class="sxs-lookup"><span data-stu-id="266d9-127">string</span></span>  | <span data-ttu-id="266d9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="266d9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="266d9-130">Accept</span><span class="sxs-lookup"><span data-stu-id="266d9-130">Accept</span></span> | <span data-ttu-id="266d9-131">string</span><span class="sxs-lookup"><span data-stu-id="266d9-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="266d9-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="266d9-132">Request body</span></span>
<span data-ttu-id="266d9-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="266d9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="266d9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="266d9-134">Response</span></span>

<span data-ttu-id="266d9-135">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [section](../resources/section.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="266d9-135">If successful, this method returns a `200 OK` response code and a collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="266d9-136">Пример</span><span class="sxs-lookup"><span data-stu-id="266d9-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="266d9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="266d9-137">Request</span></span>
<span data-ttu-id="266d9-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="266d9-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/sections
```
##### <a name="response"></a><span data-ttu-id="266d9-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="266d9-139">Response</span></span>
<span data-ttu-id="266d9-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="266d9-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-list-sections.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
