---
title: Список элементов
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: lleonard-msft
ms.openlocfilehash: 8bd0f67d6ca565dac6dfae501f5bc5c829f4db3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359103"
---
# <a name="list-members"></a><span data-ttu-id="0363f-104">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="0363f-104">List members</span></span>

> <span data-ttu-id="0363f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0363f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0363f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0363f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0363f-p103">Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="0363f-p103">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="0363f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0363f-109">Permissions</span></span>
<span data-ttu-id="0363f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0363f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0363f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0363f-112">Permission type</span></span>      | <span data-ttu-id="0363f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0363f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0363f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0363f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0363f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0363f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0363f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0363f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0363f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0363f-117">Not supported.</span></span>    |
|<span data-ttu-id="0363f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0363f-118">Application</span></span> | <span data-ttu-id="0363f-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0363f-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0363f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0363f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0363f-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0363f-121">Optional query parameters</span></span>
<span data-ttu-id="0363f-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0363f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0363f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0363f-123">Request headers</span></span>
| <span data-ttu-id="0363f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0363f-124">Name</span></span>       | <span data-ttu-id="0363f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0363f-125">Type</span></span> | <span data-ttu-id="0363f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0363f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0363f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0363f-127">Authorization</span></span>  | <span data-ttu-id="0363f-128">string</span><span class="sxs-lookup"><span data-stu-id="0363f-128">string</span></span>  | <span data-ttu-id="0363f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0363f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0363f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0363f-131">Request body</span></span>
<span data-ttu-id="0363f-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0363f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0363f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0363f-133">Response</span></span>

<span data-ttu-id="0363f-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0363f-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0363f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0363f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0363f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0363f-136">Request</span></span>
<span data-ttu-id="0363f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0363f-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="0363f-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="0363f-138">Response</span></span>
<span data-ttu-id="0363f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0363f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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