---
title: Список элементов
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: c1e58a7705abeafa56acde7e1d069a346ac3881a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805483"
---
# <a name="list-members"></a><span data-ttu-id="221e3-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="221e3-104">List members</span></span>

<span data-ttu-id="221e3-p102">Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="221e3-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="221e3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="221e3-107">Permissions</span></span>
<span data-ttu-id="221e3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="221e3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="221e3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="221e3-110">Permission type</span></span>      | <span data-ttu-id="221e3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="221e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="221e3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="221e3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="221e3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="221e3-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="221e3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="221e3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="221e3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="221e3-115">Not supported.</span></span>    |
|<span data-ttu-id="221e3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="221e3-116">Application</span></span> | <span data-ttu-id="221e3-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="221e3-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="221e3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="221e3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="221e3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="221e3-119">Optional query parameters</span></span>
<span data-ttu-id="221e3-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="221e3-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="221e3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="221e3-121">Request headers</span></span>
| <span data-ttu-id="221e3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="221e3-122">Name</span></span>       | <span data-ttu-id="221e3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="221e3-123">Type</span></span> | <span data-ttu-id="221e3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="221e3-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="221e3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="221e3-125">Authorization</span></span>  | <span data-ttu-id="221e3-126">string</span><span class="sxs-lookup"><span data-stu-id="221e3-126">string</span></span>  | <span data-ttu-id="221e3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="221e3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="221e3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="221e3-129">Request body</span></span>
<span data-ttu-id="221e3-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="221e3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="221e3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="221e3-131">Response</span></span>

<span data-ttu-id="221e3-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="221e3-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="221e3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="221e3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="221e3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="221e3-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="221e3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="221e3-135">Response</span></span>
<span data-ttu-id="221e3-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="221e3-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
