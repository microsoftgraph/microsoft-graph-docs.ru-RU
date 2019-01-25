---
title: Получение groupLifecyclePolicy
description: Получение свойств и связей, принадлежащих объекту groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 76541935c08b675913a9c7869698ebd8b5f19d38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529406"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="73613-103">Получение groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="73613-103">Get groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73613-104">Получение свойств и связей, принадлежащих объекту [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="73613-104">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73613-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73613-105">Permissions</span></span>

<span data-ttu-id="73613-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="73613-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73613-108">Permission type</span></span>      | <span data-ttu-id="73613-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73613-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73613-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73613-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73613-111">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73613-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="73613-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73613-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73613-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73613-113">Not supported</span></span> |
|<span data-ttu-id="73613-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="73613-114">Application</span></span> | <span data-ttu-id="73613-115">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73613-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73613-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73613-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73613-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73613-117">Optional query parameters</span></span>
<span data-ttu-id="73613-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73613-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73613-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73613-119">Request headers</span></span>
| <span data-ttu-id="73613-120">Имя</span><span class="sxs-lookup"><span data-stu-id="73613-120">Name</span></span> | <span data-ttu-id="73613-121">Описание</span><span class="sxs-lookup"><span data-stu-id="73613-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="73613-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73613-122">Authorization</span></span> | <span data-ttu-id="73613-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73613-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73613-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73613-125">Request body</span></span>
<span data-ttu-id="73613-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73613-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="73613-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="73613-127">Response</span></span>
<span data-ttu-id="73613-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="73613-128">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73613-129">Пример</span><span class="sxs-lookup"><span data-stu-id="73613-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="73613-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="73613-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="73613-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="73613-131">Response</span></span>

<span data-ttu-id="73613-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73613-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
