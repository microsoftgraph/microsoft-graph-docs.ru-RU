---
title: Создание groupLifecyclePolicy
description: Создает объект groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7fe5f1dd57039611d4c0378a1ce568b71a22ca28
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613409"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="ce8ab-103">Создание groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ce8ab-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="ce8ab-104">Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ce8ab-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce8ab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce8ab-105">Permissions</span></span>

<span data-ttu-id="ce8ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce8ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce8ab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce8ab-108">Permission type</span></span>      | <span data-ttu-id="ce8ab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce8ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce8ab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce8ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ce8ab-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce8ab-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce8ab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce8ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce8ab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce8ab-113">Not supported.</span></span>    |
|<span data-ttu-id="ce8ab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce8ab-114">Application</span></span> | <span data-ttu-id="ce8ab-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce8ab-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce8ab-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce8ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="ce8ab-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce8ab-117">Request headers</span></span>

| <span data-ttu-id="ce8ab-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ce8ab-118">Name</span></span> | <span data-ttu-id="ce8ab-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ce8ab-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ce8ab-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce8ab-120">Authorization</span></span> | <span data-ttu-id="ce8ab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce8ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce8ab-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce8ab-123">Content-Type</span></span>  | <span data-ttu-id="ce8ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ce8ab-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce8ab-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce8ab-125">Request body</span></span>
<span data-ttu-id="ce8ab-126">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce8ab-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ce8ab-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce8ab-127">Response</span></span>

<span data-ttu-id="ce8ab-128">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ce8ab-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce8ab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ce8ab-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ce8ab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce8ab-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="ce8ab-131">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce8ab-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ce8ab-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce8ab-132">Response</span></span>

<span data-ttu-id="ce8ab-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce8ab-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce8ab-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ce8ab-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce8ab-136">Языках</span><span class="sxs-lookup"><span data-stu-id="ce8ab-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce8ab-137">Язык</span><span class="sxs-lookup"><span data-stu-id="ce8ab-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
