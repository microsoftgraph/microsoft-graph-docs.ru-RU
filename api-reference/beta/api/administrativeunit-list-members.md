---
title: Перечисление участников
description: Используйте этот интерфейс API для получения элементов списка (пользователей и групп) в административное подразделение.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7513192986e8df482209c4f8630c8dab8450e614
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917211"
---
# <a name="list-members"></a><span data-ttu-id="d4754-103">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="d4754-103">List members</span></span>

> <span data-ttu-id="d4754-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d4754-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4754-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4754-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4754-106">Используйте этот интерфейс API для получения элементов списка (пользователей и групп) в административное подразделение.</span><span class="sxs-lookup"><span data-stu-id="d4754-106">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4754-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4754-107">Permissions</span></span>
<span data-ttu-id="d4754-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4754-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d4754-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4754-110">Permission type</span></span>      | <span data-ttu-id="d4754-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4754-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4754-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4754-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d4754-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4754-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4754-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4754-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4754-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4754-115">Not supported.</span></span>    |
|<span data-ttu-id="d4754-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4754-116">Application</span></span> | <span data-ttu-id="d4754-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4754-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d4754-118">Примечание: Для получения списка членов скрытое членство в административное подразделение, Member.Read.Hidden разрешение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d4754-118">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="d4754-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4754-119">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d4754-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4754-120">Request headers</span></span>
| <span data-ttu-id="d4754-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d4754-121">Name</span></span>      |<span data-ttu-id="d4754-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d4754-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d4754-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4754-123">Authorization</span></span>  | <span data-ttu-id="d4754-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4754-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4754-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4754-126">Request body</span></span>
<span data-ttu-id="d4754-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4754-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4754-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4754-128">Response</span></span>

<span data-ttu-id="d4754-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [пользователей](../resources/user.md) и/или [группы](../resources/group.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d4754-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="d4754-130">Вместо этого Если поместить `$ref` в конце запроса ответ будет содержать коллекцию `@odata.id` ссылки и URL-адреса для членов.</span><span class="sxs-lookup"><span data-stu-id="d4754-130">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="d4754-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4754-131">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="d4754-132">Объекты элементов списка</span><span class="sxs-lookup"><span data-stu-id="d4754-132">List member objects</span></span>
<span data-ttu-id="d4754-133">Следующий запрос будут перечислены элементы, административные единицы, возвращающий пользователи и группы.</span><span class="sxs-lookup"><span data-stu-id="d4754-133">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="d4754-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d4754-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="d4754-137">Ссылки на элементы списка</span><span class="sxs-lookup"><span data-stu-id="d4754-137">List member references</span></span>
<span data-ttu-id="d4754-138">Следующий запрос будут перечислены ссылки на элемент административные единицы, возвращающий `@odata.id` ссылки на элементы.</span><span class="sxs-lookup"><span data-stu-id="d4754-138">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="d4754-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d4754-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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
