---
title: Перечисление курсов
description: 'Получение списка объектов курсов. Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ec0bcde1e53e3dfe801a4cdafbf49572b4c812b8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042837"
---
# <a name="list-classes"></a><span data-ttu-id="e774a-104">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="e774a-104">List classes</span></span>

<span data-ttu-id="e774a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e774a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e774a-106">Извлечение коллекции ресурсов educationClass.</span><span class="sxs-lookup"><span data-stu-id="e774a-106">Retrieve a collection of educationClass resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="e774a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e774a-107">Permissions</span></span>

<span data-ttu-id="e774a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e774a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e774a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e774a-110">Permission type</span></span>                        | <span data-ttu-id="e774a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e774a-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e774a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e774a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e774a-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="e774a-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="e774a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e774a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e774a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e774a-115">Not supported.</span></span>                              |
| <span data-ttu-id="e774a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e774a-116">Application</span></span>                            | <span data-ttu-id="e774a-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e774a-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="e774a-118">При делегировании разрешений будут возвращены только ресурсы educationClass, которые пользователь проверки подлинности является участником.</span><span class="sxs-lookup"><span data-stu-id="e774a-118">When delegated permissions are used, only educationClass resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="e774a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e774a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/classes
GET /education/users/{id}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e774a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e774a-120">Optional query parameters</span></span>

<span data-ttu-id="e774a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e774a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e774a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e774a-122">Request headers</span></span>

| <span data-ttu-id="e774a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e774a-123">Header</span></span>        | <span data-ttu-id="e774a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e774a-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e774a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e774a-125">Authorization</span></span> | <span data-ttu-id="e774a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e774a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e774a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e774a-128">Request body</span></span>

<span data-ttu-id="e774a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e774a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e774a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e774a-130">Response</span></span>

<span data-ttu-id="e774a-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e774a-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e774a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e774a-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e774a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e774a-133">Request</span></span>

<span data-ttu-id="e774a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e774a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e774a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e774a-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_classes_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/classes
```

# <a name="c"></a>[<span data-ttu-id="e774a-136">C#</span><span class="sxs-lookup"><span data-stu-id="e774a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-3-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e774a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e774a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-3-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e774a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e774a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-3-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e774a-139">Java</span><span class="sxs-lookup"><span data-stu-id="e774a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e774a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e774a-140">Response</span></span>

<span data-ttu-id="e774a-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e774a-141">The following is an example of the response.</span></span>

> <span data-ttu-id="e774a-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e774a-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
