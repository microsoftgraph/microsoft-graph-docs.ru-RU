---
title: Список классов образовательных учреждений
description: Получение списка курсов учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cbd644e5994f8039a29c16f0463445d92500a865
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232034"
---
# <a name="list-classes-of-an-educationschool"></a><span data-ttu-id="e810f-103">Список классов образовательных учреждений</span><span class="sxs-lookup"><span data-stu-id="e810f-103">List classes of an educationSchool</span></span>

<span data-ttu-id="e810f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e810f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e810f-105">Получите ресурсы [educationClass,](../resources/educationclass.md) которые принадлежат [educationSchool.](../resources/educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="e810f-105">Get the [educationClass](../resources/educationclass.md) resources owned by an [educationSchool](../resources/educationschool.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e810f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e810f-106">Permissions</span></span>

<span data-ttu-id="e810f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e810f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e810f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e810f-109">Permission type</span></span>                        | <span data-ttu-id="e810f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e810f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e810f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e810f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e810f-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e810f-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="e810f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e810f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e810f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e810f-114">Not supported.</span></span>                              |
| <span data-ttu-id="e810f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e810f-115">Application</span></span>                            | <span data-ttu-id="e810f-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e810f-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e810f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e810f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/{educationSchoolId}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e810f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e810f-118">Optional query parameters</span></span>

<span data-ttu-id="e810f-119">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="e810f-119">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="e810f-120">Кроме того, для ограничения ответа можно использовать параметры и `$filter` `$count` `$search` параметры запросов.</span><span class="sxs-lookup"><span data-stu-id="e810f-120">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span>

<span data-ttu-id="e810f-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="e810f-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="e810f-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="e810f-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="e810f-123">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e810f-123">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e810f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e810f-124">Request headers</span></span>
| <span data-ttu-id="e810f-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e810f-125">Header</span></span>       | <span data-ttu-id="e810f-126">Значение</span><span class="sxs-lookup"><span data-stu-id="e810f-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e810f-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e810f-127">Authorization</span></span>  | <span data-ttu-id="e810f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e810f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e810f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e810f-130">Request body</span></span>
<span data-ttu-id="e810f-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e810f-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e810f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e810f-132">Response</span></span>
<span data-ttu-id="e810f-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e810f-133">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e810f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e810f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e810f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e810f-135">Request</span></span>
<span data-ttu-id="e810f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e810f-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e810f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e810f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
# <a name="c"></a>[<span data-ttu-id="e810f-138">C#</span><span class="sxs-lookup"><span data-stu-id="e810f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e810f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e810f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e810f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e810f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e810f-141">Java</span><span class="sxs-lookup"><span data-stu-id="e810f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e810f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e810f-142">Response</span></span>
<span data-ttu-id="e810f-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e810f-143">The following is an example of the response.</span></span> 

><span data-ttu-id="e810f-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e810f-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
