---
title: Список элементов
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
ms.openlocfilehash: 8a347603c8ed99a1f25cfd5a4c0e24fb0cd991aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079445"
---
# <a name="list-members"></a><span data-ttu-id="d823b-104">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="d823b-104">List members</span></span>

> <span data-ttu-id="d823b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d823b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d823b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d823b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d823b-p103">Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="d823b-p103">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="d823b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d823b-109">Permissions</span></span>
<span data-ttu-id="d823b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d823b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d823b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d823b-112">Permission type</span></span>      | <span data-ttu-id="d823b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d823b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d823b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d823b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d823b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d823b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d823b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d823b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d823b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d823b-117">Not supported.</span></span>    |
|<span data-ttu-id="d823b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d823b-118">Application</span></span> | <span data-ttu-id="d823b-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d823b-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d823b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d823b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d823b-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d823b-121">Optional query parameters</span></span>
<span data-ttu-id="d823b-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d823b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d823b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d823b-123">Request headers</span></span>
| <span data-ttu-id="d823b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d823b-124">Name</span></span>       | <span data-ttu-id="d823b-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d823b-125">Type</span></span> | <span data-ttu-id="d823b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d823b-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d823b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d823b-127">Authorization</span></span>  | <span data-ttu-id="d823b-128">string</span><span class="sxs-lookup"><span data-stu-id="d823b-128">string</span></span>  | <span data-ttu-id="d823b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d823b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d823b-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d823b-131">Request body</span></span>
<span data-ttu-id="d823b-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d823b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d823b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d823b-133">Response</span></span>

<span data-ttu-id="d823b-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d823b-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d823b-135">Пример</span><span class="sxs-lookup"><span data-stu-id="d823b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d823b-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d823b-136">Request</span></span>
<span data-ttu-id="d823b-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d823b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="d823b-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="d823b-138">Response</span></span>
<span data-ttu-id="d823b-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d823b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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