---
title: 'user: getMemberObjects'
description: Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 219e996bdf9b796cdd6a000b988e0f2ac73023ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509989"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="06eba-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="06eba-104">user: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06eba-p102">Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="06eba-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="06eba-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06eba-107">Permissions</span></span>
<span data-ttu-id="06eba-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06eba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="06eba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06eba-110">Permission type</span></span>      | <span data-ttu-id="06eba-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06eba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06eba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06eba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06eba-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06eba-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06eba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06eba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06eba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06eba-115">Not supported.</span></span>    |
|<span data-ttu-id="06eba-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06eba-116">Application</span></span> | <span data-ttu-id="06eba-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06eba-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06eba-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06eba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="06eba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06eba-119">Request headers</span></span>
| <span data-ttu-id="06eba-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06eba-120">Header</span></span>       | <span data-ttu-id="06eba-121">Значение</span><span class="sxs-lookup"><span data-stu-id="06eba-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06eba-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06eba-122">Authorization</span></span>  | <span data-ttu-id="06eba-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06eba-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="06eba-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06eba-125">Content-Type</span></span>  | <span data-ttu-id="06eba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06eba-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06eba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06eba-127">Request body</span></span>
<span data-ttu-id="06eba-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="06eba-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="06eba-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="06eba-129">Parameter</span></span>    | <span data-ttu-id="06eba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="06eba-130">Type</span></span>   |<span data-ttu-id="06eba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="06eba-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06eba-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="06eba-132">securityEnabledOnly</span></span>|<span data-ttu-id="06eba-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="06eba-133">Boolean</span></span>|<span data-ttu-id="06eba-p105">**true** (указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь) и **false** (указывает, что должны быть возвращены все группы, в которых состоит пользователь). Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="06eba-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="06eba-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="06eba-136">Response</span></span>

<span data-ttu-id="06eba-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию строк в тексте отклика, содержащую идентификаторы групп и ролей каталога, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="06eba-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="06eba-138">Пример</span><span class="sxs-lookup"><span data-stu-id="06eba-138">Example</span></span>
<span data-ttu-id="06eba-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="06eba-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="06eba-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="06eba-140">Request</span></span>
<span data-ttu-id="06eba-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06eba-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="06eba-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="06eba-142">Response</span></span>
<span data-ttu-id="06eba-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="06eba-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-getmemberobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
