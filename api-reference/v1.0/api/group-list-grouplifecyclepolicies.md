---
title: Перечисление groupLifecyclePolicies
description: Получает список объектов groupLifecyclePolicy, к которым принадлежит группа.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b5ff17fb3aac0b765eb9480ddccaee77a88fcf0d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726790"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="05301-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="05301-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="05301-104">Получает список объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md), к которым принадлежит группа.</span><span class="sxs-lookup"><span data-stu-id="05301-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="05301-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05301-105">Permissions</span></span>

<span data-ttu-id="05301-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05301-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05301-108">Permission type</span></span>      | <span data-ttu-id="05301-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05301-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05301-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05301-110">Delegated (work or school account)</span></span> | <span data-ttu-id="05301-111">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05301-111">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="05301-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05301-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05301-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05301-113">Not supported.</span></span>    |
|<span data-ttu-id="05301-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05301-114">Application</span></span> | <span data-ttu-id="05301-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05301-115">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05301-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05301-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05301-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="05301-117">Optional query parameters</span></span>
<span data-ttu-id="05301-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="05301-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05301-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05301-119">Request headers</span></span>
| <span data-ttu-id="05301-120">Имя</span><span class="sxs-lookup"><span data-stu-id="05301-120">Name</span></span> | <span data-ttu-id="05301-121">Описание</span><span class="sxs-lookup"><span data-stu-id="05301-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="05301-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05301-122">Authorization</span></span> | <span data-ttu-id="05301-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05301-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05301-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05301-125">Request body</span></span>
<span data-ttu-id="05301-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05301-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="05301-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="05301-127">Response</span></span>
<span data-ttu-id="05301-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05301-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="05301-129">Пример</span><span class="sxs-lookup"><span data-stu-id="05301-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="05301-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="05301-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="05301-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="05301-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="05301-132">C#</span><span class="sxs-lookup"><span data-stu-id="05301-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05301-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05301-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05301-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="05301-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="05301-135">Java</span><span class="sxs-lookup"><span data-stu-id="05301-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="05301-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="05301-136">Response</span></span>

<span data-ttu-id="05301-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05301-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

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
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
