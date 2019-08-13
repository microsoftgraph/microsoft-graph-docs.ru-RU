---
title: Перечисление groupLifecyclePolicies
description: Получает список объектов groupLifecyclePolicy, к которым принадлежит группа.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 49a82c82b04352ac76cfa8445a2682b6add2e933
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337288"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="c309c-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="c309c-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="c309c-104">Получает список объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md), к которым принадлежит группа.</span><span class="sxs-lookup"><span data-stu-id="c309c-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="c309c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c309c-105">Permissions</span></span>

<span data-ttu-id="c309c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c309c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c309c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c309c-108">Permission type</span></span>      | <span data-ttu-id="c309c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c309c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c309c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c309c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c309c-111">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c309c-111">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c309c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c309c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c309c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c309c-113">Not supported.</span></span>    |
|<span data-ttu-id="c309c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c309c-114">Application</span></span> | <span data-ttu-id="c309c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c309c-115">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c309c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c309c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c309c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c309c-117">Optional query parameters</span></span>
<span data-ttu-id="c309c-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c309c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c309c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c309c-119">Request headers</span></span>
| <span data-ttu-id="c309c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c309c-120">Name</span></span> | <span data-ttu-id="c309c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c309c-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="c309c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c309c-122">Authorization</span></span> | <span data-ttu-id="c309c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c309c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c309c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c309c-125">Request body</span></span>
<span data-ttu-id="c309c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c309c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c309c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c309c-127">Response</span></span>
<span data-ttu-id="c309c-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c309c-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c309c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c309c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c309c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c309c-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c309c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c309c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c309c-132">C#</span><span class="sxs-lookup"><span data-stu-id="c309c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c309c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c309c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c309c-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c309c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c309c-135">Java</span><span class="sxs-lookup"><span data-stu-id="c309c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c309c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c309c-136">Response</span></span>

<span data-ttu-id="c309c-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c309c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
