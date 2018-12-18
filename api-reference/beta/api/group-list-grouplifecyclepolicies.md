---
title: Перечисление groupLifecyclePolicies
description: Получает список объектов groupLifecyclePolicy, к которым принадлежит группа.
author: dkershaw10
ms.openlocfilehash: 9433716e8c2a6f91a15ca23a7aa915974d757bd7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311048"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="ace05-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="ace05-103">List groupLifecyclePolicies</span></span>

> <span data-ttu-id="ace05-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ace05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ace05-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace05-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ace05-106">Получает список объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md), к которым принадлежит группа.</span><span class="sxs-lookup"><span data-stu-id="ace05-106">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="ace05-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ace05-107">Permissions</span></span>

<span data-ttu-id="ace05-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace05-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ace05-110">Permission type</span></span>      | <span data-ttu-id="ace05-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ace05-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ace05-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ace05-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ace05-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ace05-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="ace05-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ace05-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ace05-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace05-115">Not supported.</span></span>    |
|<span data-ttu-id="ace05-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ace05-116">Application</span></span> | <span data-ttu-id="ace05-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ace05-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ace05-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ace05-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ace05-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ace05-119">Optional query parameters</span></span>
<span data-ttu-id="ace05-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ace05-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ace05-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ace05-121">Request headers</span></span>
| <span data-ttu-id="ace05-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ace05-122">Name</span></span> | <span data-ttu-id="ace05-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ace05-123">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ace05-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ace05-124">Authorization</span></span> | <span data-ttu-id="ace05-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ace05-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ace05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ace05-127">Request body</span></span>
<span data-ttu-id="ace05-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ace05-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ace05-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ace05-129">Response</span></span>
<span data-ttu-id="ace05-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ace05-130">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ace05-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ace05-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ace05-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ace05-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/groupLifecyclePolicies
```
##### <a name="response"></a><span data-ttu-id="ace05-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ace05-133">Response</span></span>

<span data-ttu-id="ace05-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ace05-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->