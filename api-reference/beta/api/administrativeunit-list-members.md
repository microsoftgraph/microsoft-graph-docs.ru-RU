---
title: Перечисление участников
description: Используйте этот интерфейс API для получения элементов списка (пользователей и групп) в административное подразделение.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aa8d70d72c5d55cac0ff8aea66d3c56b4e9f80ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517857"
---
# <a name="list-members"></a><span data-ttu-id="2ae3e-103">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="2ae3e-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ae3e-104">Используйте этот интерфейс API для получения элементов списка (пользователей и групп) в административное подразделение.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-104">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ae3e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ae3e-105">Permissions</span></span>
<span data-ttu-id="2ae3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ae3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2ae3e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ae3e-108">Permission type</span></span>      | <span data-ttu-id="2ae3e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ae3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ae3e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ae3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2ae3e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ae3e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ae3e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ae3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ae3e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-113">Not supported.</span></span>    |
|<span data-ttu-id="2ae3e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ae3e-114">Application</span></span> | <span data-ttu-id="2ae3e-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ae3e-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="2ae3e-116">Примечание: Для получения списка членов скрытое членство в административное подразделение, Member.Read.Hidden разрешение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-116">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="2ae3e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ae3e-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2ae3e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ae3e-118">Request headers</span></span>
| <span data-ttu-id="2ae3e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2ae3e-119">Name</span></span>      |<span data-ttu-id="2ae3e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2ae3e-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ae3e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ae3e-121">Authorization</span></span>  | <span data-ttu-id="2ae3e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ae3e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ae3e-124">Request body</span></span>
<span data-ttu-id="2ae3e-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ae3e-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ae3e-126">Response</span></span>

<span data-ttu-id="2ae3e-127">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [пользователей](../resources/user.md) и/или [группы](../resources/group.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-127">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="2ae3e-128">Вместо этого Если поместить `$ref` в конце запроса ответ будет содержать коллекцию `@odata.id` ссылки и URL-адреса для членов.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-128">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="2ae3e-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ae3e-129">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="2ae3e-130">Объекты элементов списка</span><span class="sxs-lookup"><span data-stu-id="2ae3e-130">List member objects</span></span>
<span data-ttu-id="2ae3e-131">Следующий запрос будут перечислены элементы, административные единицы, возвращающий пользователи и группы.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-131">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="2ae3e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2ae3e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="2ae3e-135">Ссылки на элементы списка</span><span class="sxs-lookup"><span data-stu-id="2ae3e-135">List member references</span></span>
<span data-ttu-id="2ae3e-136">Следующий запрос будут перечислены ссылки на элемент административные единицы, возвращающий `@odata.id` ссылки на элементы.</span><span class="sxs-lookup"><span data-stu-id="2ae3e-136">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="2ae3e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2ae3e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-list-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
