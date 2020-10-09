---
title: Перечисление groupLifecyclePolicies
description: Получает список объектов groupLifecyclePolicy, к которым принадлежит группа.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 26561000d59e820d7658c5d55b9e92fe6b5b72fb
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402809"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="26486-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="26486-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="26486-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26486-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26486-105">Получает список объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md), к которым принадлежит группа.</span><span class="sxs-lookup"><span data-stu-id="26486-105">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="26486-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26486-106">Permissions</span></span>

<span data-ttu-id="26486-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26486-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26486-109">Permission type</span></span>      | <span data-ttu-id="26486-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26486-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26486-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26486-111">Delegated (work or school account)</span></span> | <span data-ttu-id="26486-112">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26486-112">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="26486-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26486-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26486-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26486-114">Not supported.</span></span>    |
|<span data-ttu-id="26486-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26486-115">Application</span></span> | <span data-ttu-id="26486-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26486-116">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26486-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26486-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="26486-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26486-118">Optional query parameters</span></span>
<span data-ttu-id="26486-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="26486-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26486-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26486-120">Request headers</span></span>
| <span data-ttu-id="26486-121">Имя</span><span class="sxs-lookup"><span data-stu-id="26486-121">Name</span></span> | <span data-ttu-id="26486-122">Описание</span><span class="sxs-lookup"><span data-stu-id="26486-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="26486-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26486-123">Authorization</span></span> | <span data-ttu-id="26486-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26486-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26486-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26486-126">Request body</span></span>
<span data-ttu-id="26486-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26486-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="26486-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="26486-128">Response</span></span>
<span data-ttu-id="26486-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26486-129">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26486-130">Пример</span><span class="sxs-lookup"><span data-stu-id="26486-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="26486-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="26486-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="26486-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="26486-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="26486-133">C#</span><span class="sxs-lookup"><span data-stu-id="26486-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26486-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26486-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26486-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26486-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26486-136">Java</span><span class="sxs-lookup"><span data-stu-id="26486-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="26486-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="26486-137">Response</span></span>

<span data-ttu-id="26486-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26486-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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