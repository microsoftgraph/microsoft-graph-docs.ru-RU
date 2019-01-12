---
title: 'user: getMemberObjects'
description: Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b737ee5115060d02ee476b9bd0f1af4a6424e12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978153"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="f6d5c-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="f6d5c-104">user: getMemberObjects</span></span>
<span data-ttu-id="f6d5c-p102">Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6d5c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6d5c-107">Permissions</span></span>
<span data-ttu-id="f6d5c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6d5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f6d5c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6d5c-110">Permission type</span></span>      | <span data-ttu-id="f6d5c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6d5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6d5c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6d5c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f6d5c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6d5c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6d5c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6d5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6d5c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-115">Not supported.</span></span>    |
|<span data-ttu-id="f6d5c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6d5c-116">Application</span></span> | <span data-ttu-id="f6d5c-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d5c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6d5c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6d5c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="f6d5c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6d5c-119">Request headers</span></span>
| <span data-ttu-id="f6d5c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6d5c-120">Header</span></span>       | <span data-ttu-id="f6d5c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f6d5c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6d5c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6d5c-122">Authorization</span></span>  | <span data-ttu-id="f6d5c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f6d5c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6d5c-125">Content-Type</span></span>  | <span data-ttu-id="f6d5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6d5c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6d5c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6d5c-127">Request body</span></span>
<span data-ttu-id="f6d5c-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f6d5c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="f6d5c-129">Parameter</span></span>    | <span data-ttu-id="f6d5c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f6d5c-130">Type</span></span>   |<span data-ttu-id="f6d5c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f6d5c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6d5c-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f6d5c-132">securityEnabledOnly</span></span>|<span data-ttu-id="f6d5c-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="f6d5c-133">Boolean</span></span>|<span data-ttu-id="f6d5c-p105">Значение **true** указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь. Значение **false** указывает, что должны быть возвращены все группы и роли каталога, участником которых является пользователь. Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="f6d5c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6d5c-136">Response</span></span>

<span data-ttu-id="f6d5c-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию строк в тексте отклика, содержащую идентификаторы групп и ролей каталога, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="f6d5c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f6d5c-138">Example</span></span>
<span data-ttu-id="f6d5c-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f6d5c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6d5c-140">Request</span></span>
<span data-ttu-id="f6d5c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="f6d5c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6d5c-142">Response</span></span>
<span data-ttu-id="f6d5c-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f6d5c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
