---
title: Список участников
description: Используйте этот API для получения списка участников (пользователя и группы) в административном подразделении.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 873bf5b812be584725b515aa6f23505bd85cea42
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438843"
---
# <a name="list-members"></a><span data-ttu-id="e0a9e-103">Список участников</span><span class="sxs-lookup"><span data-stu-id="e0a9e-103">List members</span></span>

<span data-ttu-id="e0a9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0a9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0a9e-105">Используйте этот API для получения списка участников (пользователя и группы) в административном подразделении.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-105">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0a9e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a9e-106">Permissions</span></span>
<span data-ttu-id="e0a9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0a9e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a9e-109">Permission type</span></span>      | <span data-ttu-id="e0a9e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0a9e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0a9e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0a9e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0a9e-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0a9e-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0a9e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0a9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0a9e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-114">Not supported.</span></span>    |
|<span data-ttu-id="e0a9e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e0a9e-115">Application</span></span> | <span data-ttu-id="e0a9e-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0a9e-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e0a9e-117">Примечание. Чтобы перечислить членов скрытого членства в административном подразделении, требуется разрешение Member.Read.Hidden.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-117">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e0a9e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0a9e-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e0a9e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0a9e-119">Request headers</span></span>
| <span data-ttu-id="e0a9e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e0a9e-120">Name</span></span>      |<span data-ttu-id="e0a9e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e0a9e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0a9e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0a9e-122">Authorization</span></span>  | <span data-ttu-id="e0a9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0a9e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0a9e-125">Request body</span></span>
<span data-ttu-id="e0a9e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0a9e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0a9e-127">Response</span></span>

<span data-ttu-id="e0a9e-128">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов пользователей и/или групп в `200 OK` тексте отклика. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="e0a9e-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="e0a9e-129">Вместо этого, если вы поместите в конце запроса, ответ будет содержать коллекцию ссылок `$ref` `@odata.id` и URL-адресов для участников.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-129">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="e0a9e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e0a9e-130">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="e0a9e-131">Объекты участников списка</span><span class="sxs-lookup"><span data-stu-id="e0a9e-131">List member objects</span></span>
<span data-ttu-id="e0a9e-132">В следующем запросе будут перечисляться члены административного подразделения, возвращающие коллекцию пользователей и/или групп.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-132">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="e0a9e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="e0a9e-136">Ссылки на членов списка</span><span class="sxs-lookup"><span data-stu-id="e0a9e-136">List member references</span></span>
<span data-ttu-id="e0a9e-137">Следующий запрос будет перечислять ссылки членов административного подразделения, возвращая коллекцию ссылок `@odata.id` на членов.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-137">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="e0a9e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0a9e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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


