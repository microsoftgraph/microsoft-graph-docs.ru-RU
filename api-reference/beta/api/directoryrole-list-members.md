---
title: Список элементов
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4365408309a8d87387da76695257207f03bf5ce5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519579"
---
# <a name="list-members"></a><span data-ttu-id="9eb83-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="9eb83-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9eb83-p102">Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="9eb83-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="9eb83-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9eb83-107">Permissions</span></span>
<span data-ttu-id="9eb83-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eb83-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9eb83-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9eb83-110">Permission type</span></span>      | <span data-ttu-id="9eb83-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9eb83-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9eb83-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9eb83-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9eb83-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9eb83-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9eb83-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9eb83-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eb83-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eb83-115">Not supported.</span></span>    |
|<span data-ttu-id="9eb83-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9eb83-116">Application</span></span> | <span data-ttu-id="9eb83-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9eb83-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eb83-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9eb83-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9eb83-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9eb83-119">Optional query parameters</span></span>
<span data-ttu-id="9eb83-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9eb83-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9eb83-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9eb83-121">Request headers</span></span>
| <span data-ttu-id="9eb83-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9eb83-122">Name</span></span>       | <span data-ttu-id="9eb83-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9eb83-123">Type</span></span> | <span data-ttu-id="9eb83-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9eb83-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9eb83-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9eb83-125">Authorization</span></span>  | <span data-ttu-id="9eb83-126">string</span><span class="sxs-lookup"><span data-stu-id="9eb83-126">string</span></span>  | <span data-ttu-id="9eb83-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9eb83-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9eb83-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9eb83-129">Request body</span></span>
<span data-ttu-id="9eb83-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9eb83-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9eb83-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eb83-131">Response</span></span>

<span data-ttu-id="9eb83-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9eb83-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9eb83-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9eb83-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9eb83-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9eb83-134">Request</span></span>
<span data-ttu-id="9eb83-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9eb83-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="9eb83-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9eb83-136">Response</span></span>
<span data-ttu-id="9eb83-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9eb83-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-list-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
