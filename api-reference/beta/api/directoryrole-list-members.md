---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 087124dcbf0e612a4b6a6028c871b622a1df0ca1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590359"
---
# <a name="list-members"></a><span data-ttu-id="ba579-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="ba579-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba579-105">Получение списка пользователей, которым назначена роль каталога.</span><span class="sxs-lookup"><span data-stu-id="ba579-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="ba579-106">Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="ba579-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba579-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba579-107">Permissions</span></span>
<span data-ttu-id="ba579-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba579-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ba579-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba579-110">Permission type</span></span>      | <span data-ttu-id="ba579-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba579-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba579-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba579-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba579-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba579-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ba579-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba579-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba579-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba579-115">Not supported.</span></span>    |
|<span data-ttu-id="ba579-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba579-116">Application</span></span> | <span data-ttu-id="ba579-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba579-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba579-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba579-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ba579-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba579-119">Optional query parameters</span></span>
<span data-ttu-id="ba579-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ba579-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ba579-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba579-121">Request headers</span></span>
| <span data-ttu-id="ba579-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ba579-122">Name</span></span>       | <span data-ttu-id="ba579-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ba579-123">Type</span></span> | <span data-ttu-id="ba579-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ba579-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ba579-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba579-125">Authorization</span></span>  | <span data-ttu-id="ba579-126">string</span><span class="sxs-lookup"><span data-stu-id="ba579-126">string</span></span>  | <span data-ttu-id="ba579-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba579-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba579-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba579-129">Request body</span></span>
<span data-ttu-id="ba579-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba579-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba579-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba579-131">Response</span></span>

<span data-ttu-id="ba579-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba579-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba579-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ba579-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba579-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba579-134">Request</span></span>
<span data-ttu-id="ba579-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba579-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="ba579-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba579-136">Response</span></span>
<span data-ttu-id="ba579-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba579-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ba579-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ba579-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ba579-141">Языках</span><span class="sxs-lookup"><span data-stu-id="ba579-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba579-142">Язык</span><span class="sxs-lookup"><span data-stu-id="ba579-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
