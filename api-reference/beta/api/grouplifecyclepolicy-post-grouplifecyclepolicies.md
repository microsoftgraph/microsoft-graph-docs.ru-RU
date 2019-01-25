---
title: Создание groupLifecyclePolicy
description: Создает объект groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 9ba07aeaa0d9aabf63fb6d8598fb238e03c3586d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522681"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="a5d37-103">Создание groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a5d37-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5d37-104">Создает объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a5d37-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5d37-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5d37-105">Permissions</span></span>

<span data-ttu-id="a5d37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5d37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5d37-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5d37-108">Permission type</span></span>      | <span data-ttu-id="a5d37-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5d37-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5d37-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5d37-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5d37-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d37-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5d37-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5d37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5d37-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a5d37-113">Not supported</span></span> |
|<span data-ttu-id="a5d37-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5d37-114">Application</span></span> |  <span data-ttu-id="a5d37-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d37-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5d37-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5d37-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="a5d37-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5d37-117">Request headers</span></span>

| <span data-ttu-id="a5d37-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a5d37-118">Name</span></span> | <span data-ttu-id="a5d37-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a5d37-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a5d37-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5d37-120">Authorization</span></span> | <span data-ttu-id="a5d37-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5d37-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5d37-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5d37-123">Content-Type</span></span>  | <span data-ttu-id="a5d37-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a5d37-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5d37-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5d37-125">Request body</span></span>
<span data-ttu-id="a5d37-126">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5d37-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a5d37-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5d37-127">Response</span></span>

<span data-ttu-id="a5d37-128">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5d37-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5d37-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a5d37-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5d37-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5d37-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="a5d37-131">В теле запроса предоставьте описание объекта [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5d37-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a5d37-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5d37-132">Response</span></span>

<span data-ttu-id="a5d37-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5d37-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
