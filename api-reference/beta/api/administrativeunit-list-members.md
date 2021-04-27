---
title: Список участников
description: Используйте этот API для получения списка участников (пользователя и группы) в административном подразделении.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 294cbdb96f44de5028e2f41fdb9c2c7caf9d186b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048262"
---
# <a name="list-members"></a><span data-ttu-id="b04cf-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="b04cf-103">List members</span></span>

<span data-ttu-id="b04cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b04cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b04cf-105">Используйте этот API для получения списка участников (пользователя и группы) в административном подразделении.</span><span class="sxs-lookup"><span data-stu-id="b04cf-105">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="b04cf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b04cf-106">Permissions</span></span>
<span data-ttu-id="b04cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b04cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b04cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b04cf-109">Permission type</span></span>      | <span data-ttu-id="b04cf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b04cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b04cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b04cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b04cf-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b04cf-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b04cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b04cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b04cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b04cf-114">Not supported.</span></span>    |
|<span data-ttu-id="b04cf-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b04cf-115">Application</span></span> | <span data-ttu-id="b04cf-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b04cf-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="b04cf-117">Примечание. Чтобы перечислить членов скрытого членства в административном подразделении, требуется разрешение Member.Read.Hidden.</span><span class="sxs-lookup"><span data-stu-id="b04cf-117">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b04cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b04cf-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b04cf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b04cf-119">Request headers</span></span>
| <span data-ttu-id="b04cf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b04cf-120">Name</span></span>      |<span data-ttu-id="b04cf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b04cf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b04cf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b04cf-122">Authorization</span></span>  | <span data-ttu-id="b04cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b04cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b04cf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b04cf-125">Request body</span></span>
<span data-ttu-id="b04cf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b04cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b04cf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b04cf-127">Response</span></span>

<span data-ttu-id="b04cf-128">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов пользователей и/или групп в `200 OK` тексте отклика. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="b04cf-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="b04cf-129">Вместо этого, если вы поместите в конце запроса, ответ будет содержать коллекцию ссылок `$ref` `@odata.id` и URL-адресов для участников.</span><span class="sxs-lookup"><span data-stu-id="b04cf-129">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="b04cf-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="b04cf-130">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="b04cf-131">Объекты участников списка</span><span class="sxs-lookup"><span data-stu-id="b04cf-131">List member objects</span></span>
<span data-ttu-id="b04cf-132">В следующем запросе будут перечисляться члены административного подразделения, возвращающие коллекцию пользователей и/или групп.</span><span class="sxs-lookup"><span data-stu-id="b04cf-132">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="b04cf-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b04cf-133">Here is an example of the response.</span></span> <span data-ttu-id="b04cf-134">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b04cf-134">Note: The response object shown here might be shortened for readability.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="b04cf-135">Ссылки на членов списка</span><span class="sxs-lookup"><span data-stu-id="b04cf-135">List member references</span></span>
<span data-ttu-id="b04cf-136">Следующий запрос будет перечислять ссылки членов административного подразделения, возвращая коллекцию ссылок `@odata.id` на членов.</span><span class="sxs-lookup"><span data-stu-id="b04cf-136">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="b04cf-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b04cf-137">Here is an example of the response.</span></span> <span data-ttu-id="b04cf-138">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b04cf-138">Note: The response object shown here might be shortened for readability.</span></span>
 
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


