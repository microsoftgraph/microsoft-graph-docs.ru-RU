---
title: Список элементов
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4365408309a8d87387da76695257207f03bf5ce5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454794"
---
# <a name="list-members"></a><span data-ttu-id="2db9d-104">Список членов</span><span class="sxs-lookup"><span data-stu-id="2db9d-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2db9d-105">Получение списка пользователей, которым назначена роль каталога.</span><span class="sxs-lookup"><span data-stu-id="2db9d-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="2db9d-106">Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="2db9d-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="2db9d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2db9d-107">Permissions</span></span>
<span data-ttu-id="2db9d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2db9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2db9d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2db9d-110">Permission type</span></span>      | <span data-ttu-id="2db9d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2db9d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2db9d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2db9d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2db9d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2db9d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2db9d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2db9d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2db9d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2db9d-115">Not supported.</span></span>    |
|<span data-ttu-id="2db9d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2db9d-116">Application</span></span> | <span data-ttu-id="2db9d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2db9d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2db9d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2db9d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2db9d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2db9d-119">Optional query parameters</span></span>
<span data-ttu-id="2db9d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2db9d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2db9d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2db9d-121">Request headers</span></span>
| <span data-ttu-id="2db9d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2db9d-122">Name</span></span>       | <span data-ttu-id="2db9d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2db9d-123">Type</span></span> | <span data-ttu-id="2db9d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2db9d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2db9d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2db9d-125">Authorization</span></span>  | <span data-ttu-id="2db9d-126">string</span><span class="sxs-lookup"><span data-stu-id="2db9d-126">string</span></span>  | <span data-ttu-id="2db9d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2db9d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2db9d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2db9d-129">Request body</span></span>
<span data-ttu-id="2db9d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2db9d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2db9d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2db9d-131">Response</span></span>

<span data-ttu-id="2db9d-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2db9d-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2db9d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2db9d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2db9d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2db9d-134">Request</span></span>
<span data-ttu-id="2db9d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2db9d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="2db9d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2db9d-136">Response</span></span>
<span data-ttu-id="2db9d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2db9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
