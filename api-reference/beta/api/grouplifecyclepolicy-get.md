---
title: Получение groupLifecyclePolicy
description: Получение свойств и связей, принадлежащих объекту groupLifecyclePolicies.
author: dkershaw10
ms.openlocfilehash: ef239385766b33c4a03576200c6c9abf3938c25a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312525"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="982e0-103">Получение groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="982e0-103">Get groupLifecyclePolicy</span></span>

> <span data-ttu-id="982e0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="982e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="982e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="982e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="982e0-106">Получение свойств и связей, принадлежащих объекту [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="982e0-106">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="982e0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="982e0-107">Permissions</span></span>

<span data-ttu-id="982e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="982e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="982e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="982e0-110">Permission type</span></span>      | <span data-ttu-id="982e0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="982e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="982e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="982e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="982e0-113">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="982e0-113">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="982e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="982e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="982e0-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="982e0-115">Not supported</span></span> |
|<span data-ttu-id="982e0-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="982e0-116">Application</span></span> | <span data-ttu-id="982e0-117">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="982e0-117">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="982e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="982e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="982e0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="982e0-119">Optional query parameters</span></span>
<span data-ttu-id="982e0-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="982e0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="982e0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="982e0-121">Request headers</span></span>
| <span data-ttu-id="982e0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="982e0-122">Name</span></span> | <span data-ttu-id="982e0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="982e0-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="982e0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="982e0-124">Authorization</span></span> | <span data-ttu-id="982e0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="982e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="982e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="982e0-127">Request body</span></span>
<span data-ttu-id="982e0-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="982e0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="982e0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="982e0-129">Response</span></span>
<span data-ttu-id="982e0-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="982e0-130">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="982e0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="982e0-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="982e0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="982e0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="982e0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="982e0-133">Response</span></span>

<span data-ttu-id="982e0-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="982e0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->