---
title: Список taughtClasses
description: Получите ресурсы educationClass из свойства навигации taughtClasses.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a82e647f8c2db6859142c5de5cba619371248add
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475425"
---
# <a name="list-taughtclasses"></a><span data-ttu-id="5b23f-103">Список taughtClasses</span><span class="sxs-lookup"><span data-stu-id="5b23f-103">List taughtClasses</span></span>

<span data-ttu-id="5b23f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b23f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b23f-105">Получите [ресурсы educationClass,](../resources/educationclass.md) которые принадлежат [educationUser.](../resources/educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="5b23f-105">Get the [educationClass](../resources/educationclass.md) resources owned by an [educationUser](../resources/educationuser.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b23f-106">Разрешения:</span><span class="sxs-lookup"><span data-stu-id="5b23f-106">Permissions</span></span>

<span data-ttu-id="5b23f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b23f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b23f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b23f-109">Permission type</span></span>                        | <span data-ttu-id="5b23f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b23f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5b23f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b23f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b23f-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="5b23f-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="5b23f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b23f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b23f-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b23f-114">Not supported</span></span>                               |
| <span data-ttu-id="5b23f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b23f-115">Application</span></span>                            | <span data-ttu-id="5b23f-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b23f-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="5b23f-117">Обратите внимание, что при делегировании маркера пользователи могут видеть только сведения о своих классах.</span><span class="sxs-lookup"><span data-stu-id="5b23f-117">Note that if the delegated token is used, users can only see information about their own classes.</span></span>

## <a name="http-request"></a><span data-ttu-id="5b23f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b23f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/me/taughtClasses
GET /education/users/{educationUserId}/taughtClasses
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b23f-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5b23f-119">Optional query parameters</span></span>

<span data-ttu-id="5b23f-120">С помощью параметра `$orderby` запросов OData можно сортировать группы в организации по значениям **displayName**, как показано в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="5b23f-120">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="5b23f-121">Кроме того, для ограничения ответа можно использовать параметры и `$filter` `$count` `$search` параметры запросов.</span><span class="sxs-lookup"><span data-stu-id="5b23f-121">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span>

<span data-ttu-id="5b23f-122">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="5b23f-122">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="5b23f-123">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="5b23f-123">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="5b23f-124">Дополнительные сведения о параметрах запроса OData см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5b23f-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b23f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b23f-125">Request headers</span></span>

| <span data-ttu-id="5b23f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="5b23f-126">Name</span></span>          | <span data-ttu-id="5b23f-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5b23f-127">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5b23f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b23f-128">Authorization</span></span> | <span data-ttu-id="5b23f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b23f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b23f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b23f-131">Request body</span></span>

<span data-ttu-id="5b23f-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b23f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b23f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b23f-133">Response</span></span>

<span data-ttu-id="5b23f-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b23f-134">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b23f-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b23f-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b23f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b23f-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5b23f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b23f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_educationclass"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/taughtClasses
```
# <a name="c"></a>[<span data-ttu-id="5b23f-138">C#</span><span class="sxs-lookup"><span data-stu-id="5b23f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b23f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b23f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b23f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b23f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b23f-141">Java</span><span class="sxs-lookup"><span data-stu-id="5b23f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b23f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b23f-142">Response</span></span>

> <span data-ttu-id="5b23f-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5b23f-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationClass)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
      "displayName": "String",
      "mailNickname": "String",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "String",
      "externalName": "String",
      "externalId": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "grade": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      }
    }
  ]
}
```
