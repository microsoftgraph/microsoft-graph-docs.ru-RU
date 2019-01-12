---
title: Список элементов
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad27b5d4a56bee9e149b9f6de87271a86e9945e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970810"
---
# <a name="list-members"></a><span data-ttu-id="4f0b0-104">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="4f0b0-104">List members</span></span>

> <span data-ttu-id="4f0b0-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f0b0-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f0b0-p103">Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-p103">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="4f0b0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f0b0-109">Permissions</span></span>
<span data-ttu-id="4f0b0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f0b0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4f0b0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f0b0-112">Permission type</span></span>      | <span data-ttu-id="4f0b0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f0b0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f0b0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f0b0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4f0b0-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f0b0-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4f0b0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f0b0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f0b0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-117">Not supported.</span></span>    |
|<span data-ttu-id="4f0b0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f0b0-118">Application</span></span> | <span data-ttu-id="4f0b0-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f0b0-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f0b0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f0b0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4f0b0-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f0b0-121">Optional query parameters</span></span>
<span data-ttu-id="4f0b0-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4f0b0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f0b0-123">Request headers</span></span>
| <span data-ttu-id="4f0b0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4f0b0-124">Name</span></span>       | <span data-ttu-id="4f0b0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4f0b0-125">Type</span></span> | <span data-ttu-id="4f0b0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4f0b0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f0b0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f0b0-127">Authorization</span></span>  | <span data-ttu-id="4f0b0-128">string</span><span class="sxs-lookup"><span data-stu-id="4f0b0-128">string</span></span>  | <span data-ttu-id="4f0b0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f0b0-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f0b0-131">Request body</span></span>
<span data-ttu-id="4f0b0-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f0b0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0b0-133">Response</span></span>

<span data-ttu-id="4f0b0-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4f0b0-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4f0b0-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f0b0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f0b0-136">Request</span></span>
<span data-ttu-id="4f0b0-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="4f0b0-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f0b0-138">Response</span></span>
<span data-ttu-id="4f0b0-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4f0b0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
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
