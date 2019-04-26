---
title: Список участников
description: Используйте этот API, чтобы получить список Members (User и Group) в административной единице.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b156079035b2f2332d81e018eba40bced41d9aee
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322798"
---
# <a name="list-members"></a><span data-ttu-id="d9e2f-103">Список элементов</span><span class="sxs-lookup"><span data-stu-id="d9e2f-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9e2f-104">Используйте этот API, чтобы получить список Members (User и Group) в административной единице.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-104">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9e2f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9e2f-105">Permissions</span></span>
<span data-ttu-id="d9e2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d9e2f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9e2f-108">Permission type</span></span>      | <span data-ttu-id="d9e2f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9e2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9e2f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9e2f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d9e2f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d9e2f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d9e2f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9e2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9e2f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-113">Not supported.</span></span>    |
|<span data-ttu-id="d9e2f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9e2f-114">Application</span></span> | <span data-ttu-id="d9e2f-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e2f-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d9e2f-116">Note: чтобы получить список членов скрытого членства в административной единице, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-116">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="d9e2f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9e2f-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d9e2f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9e2f-118">Request headers</span></span>
| <span data-ttu-id="d9e2f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d9e2f-119">Name</span></span>      |<span data-ttu-id="d9e2f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d9e2f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d9e2f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9e2f-121">Authorization</span></span>  | <span data-ttu-id="d9e2f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9e2f-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9e2f-124">Request body</span></span>
<span data-ttu-id="d9e2f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9e2f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9e2f-126">Response</span></span>

<span data-ttu-id="d9e2f-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [User](../resources/user.md) и/или [Group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-127">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="d9e2f-128">Вместо этого, если вы `$ref` помещаете в конец запроса, ответ будет содержать коллекцию `@odata.id` ссылок/URL-адресов для членов.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-128">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="d9e2f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="d9e2f-129">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="d9e2f-130">Список объектов Member</span><span class="sxs-lookup"><span data-stu-id="d9e2f-130">List member objects</span></span>
<span data-ttu-id="d9e2f-131">Следующий запрос выведет список членов административной единицы, возвращая коллекцию пользователей и/или групп.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-131">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="d9e2f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a><span data-ttu-id="d9e2f-135">Ссылки на элементы списка</span><span class="sxs-lookup"><span data-stu-id="d9e2f-135">List member references</span></span>
<span data-ttu-id="d9e2f-136">Следующий запрос выведет список ссылок на элементы административной единицы, возвращая коллекцию `@odata.id` ссылок на элементы.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-136">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="d9e2f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9e2f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
