---
title: Перечисление groupLifecyclePolicies
description: Получает список объектов groupLifecyclePolicy, к которым принадлежит группа.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 98b9ddd448a78c025b3396c22d7da86c17913395
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592999"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="38b5e-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="38b5e-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="38b5e-104">Получает список объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md), к которым принадлежит группа.</span><span class="sxs-lookup"><span data-stu-id="38b5e-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="38b5e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38b5e-105">Permissions</span></span>

<span data-ttu-id="38b5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38b5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38b5e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38b5e-108">Permission type</span></span>      | <span data-ttu-id="38b5e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38b5e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38b5e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38b5e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="38b5e-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="38b5e-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="38b5e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38b5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38b5e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38b5e-113">Not supported.</span></span>    |
|<span data-ttu-id="38b5e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38b5e-114">Application</span></span> | <span data-ttu-id="38b5e-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="38b5e-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38b5e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38b5e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="38b5e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38b5e-117">Optional query parameters</span></span>
<span data-ttu-id="38b5e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="38b5e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38b5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38b5e-119">Request headers</span></span>
| <span data-ttu-id="38b5e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="38b5e-120">Name</span></span> | <span data-ttu-id="38b5e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="38b5e-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="38b5e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38b5e-122">Authorization</span></span> | <span data-ttu-id="38b5e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38b5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38b5e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38b5e-125">Request body</span></span>
<span data-ttu-id="38b5e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38b5e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="38b5e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="38b5e-127">Response</span></span>
<span data-ttu-id="38b5e-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="38b5e-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38b5e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="38b5e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38b5e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="38b5e-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="38b5e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="38b5e-131">Response</span></span>

<span data-ttu-id="38b5e-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38b5e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="38b5e-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="38b5e-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38b5e-135">Языках</span><span class="sxs-lookup"><span data-stu-id="38b5e-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38b5e-136">Язык</span><span class="sxs-lookup"><span data-stu-id="38b5e-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_grouplifecyclepolicies-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
