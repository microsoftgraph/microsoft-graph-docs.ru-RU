---
title: Получение groupLifecyclePolicy
description: Получение свойств и связей, принадлежащих объекту groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0b4d29ca8a08c2ec805549e6f10da4ac268771a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566131"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="7d405-103">Получение groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7d405-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="7d405-104">Получение свойств и связей, принадлежащих объекту [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7d405-104">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d405-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d405-105">Permissions</span></span>

<span data-ttu-id="7d405-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d405-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d405-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d405-108">Permission type</span></span>      | <span data-ttu-id="7d405-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d405-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d405-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d405-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d405-111">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d405-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="7d405-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d405-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d405-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d405-113">Not supported.</span></span>    |
|<span data-ttu-id="7d405-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d405-114">Application</span></span> | <span data-ttu-id="7d405-115">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d405-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d405-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d405-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d405-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d405-117">Optional query parameters</span></span>
<span data-ttu-id="7d405-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d405-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d405-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d405-119">Request headers</span></span>
| <span data-ttu-id="7d405-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7d405-120">Name</span></span> | <span data-ttu-id="7d405-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7d405-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="7d405-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d405-122">Authorization</span></span> | <span data-ttu-id="7d405-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d405-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d405-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d405-125">Request body</span></span>
<span data-ttu-id="7d405-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d405-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7d405-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d405-127">Response</span></span>
<span data-ttu-id="7d405-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7d405-128">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d405-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7d405-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7d405-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d405-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="7d405-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d405-131">Response</span></span>

<span data-ttu-id="7d405-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d405-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
