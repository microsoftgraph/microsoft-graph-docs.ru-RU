---
title: Перечисление курсов
description: 'Получение списка объектов курсов. Примечание. Если используется делегированный маркер, участники могут видеть сведения только о своих курсах. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 50e5752431a42792497142fd6b9fcc0fd299df71
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458220"
---
# <a name="list-classes"></a><span data-ttu-id="02665-104">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="02665-104">List classes</span></span>

<span data-ttu-id="02665-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02665-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02665-106">Получение коллекции ресурсов educationClass.</span><span class="sxs-lookup"><span data-stu-id="02665-106">Retrieve a collection of educationClass resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="02665-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02665-107">Permissions</span></span>

<span data-ttu-id="02665-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02665-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02665-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02665-110">Permission type</span></span>                        | <span data-ttu-id="02665-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02665-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="02665-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02665-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="02665-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="02665-113">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="02665-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02665-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02665-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02665-115">Not supported.</span></span>                              |
| <span data-ttu-id="02665-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02665-116">Application</span></span>                            | <span data-ttu-id="02665-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02665-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="02665-118">При использовании делегированных разрешений возвращаются только те ресурсы educationClass, которые является членом пользователя проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="02665-118">When delegated permissions are used, only educationClass resources that the authentication user is a member will be returned.</span></span>

## <a name="http-request"></a><span data-ttu-id="02665-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02665-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/classes
GET /education/users/{id}/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02665-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="02665-120">Optional query parameters</span></span>

<span data-ttu-id="02665-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="02665-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02665-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02665-122">Request headers</span></span>

| <span data-ttu-id="02665-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02665-123">Header</span></span>        | <span data-ttu-id="02665-124">Значение</span><span class="sxs-lookup"><span data-stu-id="02665-124">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="02665-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02665-125">Authorization</span></span> | <span data-ttu-id="02665-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02665-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02665-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02665-128">Request body</span></span>

<span data-ttu-id="02665-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02665-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02665-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="02665-130">Response</span></span>

<span data-ttu-id="02665-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="02665-131">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02665-132">Пример</span><span class="sxs-lookup"><span data-stu-id="02665-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="02665-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="02665-133">Request</span></span>

<span data-ttu-id="02665-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02665-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02665-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="02665-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/classes
```

# <a name="c"></a>[<span data-ttu-id="02665-136">C#</span><span class="sxs-lookup"><span data-stu-id="02665-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02665-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02665-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02665-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02665-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02665-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="02665-139">Response</span></span>

<span data-ttu-id="02665-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="02665-140">The following is an example of the response.</span></span>

> <span data-ttu-id="02665-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02665-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
