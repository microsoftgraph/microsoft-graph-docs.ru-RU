---
title: Перечисление groupLifecyclePolicies
description: Получает список объектов groupLifecyclePolicy, к которым принадлежит группа.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: c4c63497b82c23bbefb2eee6bae5fc0ec30c4849
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419466"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="a9476-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="a9476-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="a9476-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a9476-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9476-105">Получает список объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md), к которым принадлежит группа.</span><span class="sxs-lookup"><span data-stu-id="a9476-105">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9476-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9476-106">Permissions</span></span>

<span data-ttu-id="a9476-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9476-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9476-109">Permission type</span></span>      | <span data-ttu-id="a9476-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9476-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9476-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9476-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9476-112">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9476-112">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a9476-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9476-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9476-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9476-114">Not supported.</span></span>    |
|<span data-ttu-id="a9476-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9476-115">Application</span></span> | <span data-ttu-id="a9476-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9476-116">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9476-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9476-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a9476-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a9476-118">Optional query parameters</span></span>
<span data-ttu-id="a9476-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a9476-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9476-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9476-120">Request headers</span></span>
| <span data-ttu-id="a9476-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a9476-121">Name</span></span> | <span data-ttu-id="a9476-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a9476-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="a9476-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9476-123">Authorization</span></span> | <span data-ttu-id="a9476-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9476-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9476-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9476-126">Request body</span></span>
<span data-ttu-id="a9476-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9476-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a9476-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9476-128">Response</span></span>
<span data-ttu-id="a9476-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a9476-129">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9476-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a9476-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a9476-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9476-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a9476-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9476-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="a9476-133">C#</span><span class="sxs-lookup"><span data-stu-id="a9476-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9476-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9476-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9476-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9476-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a9476-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9476-136">Response</span></span>

<span data-ttu-id="a9476-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9476-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 227

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
