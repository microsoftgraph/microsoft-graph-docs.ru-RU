---
title: 'user: getMemberObjects'
description: Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.
ms.openlocfilehash: 337bf806be40b5e0af3600ea5fbeab5e94c079b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074601"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="de53f-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="de53f-104">user: getMemberObjects</span></span>

> <span data-ttu-id="de53f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de53f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de53f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de53f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de53f-p103">Возвращение всех групп, ролей каталога и административных подразделений, в которых состоит пользователь. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="de53f-p103">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="de53f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de53f-109">Permissions</span></span>
<span data-ttu-id="de53f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de53f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="de53f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de53f-112">Permission type</span></span>      | <span data-ttu-id="de53f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de53f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de53f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de53f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="de53f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="de53f-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="de53f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de53f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de53f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de53f-117">Not supported.</span></span>    |
|<span data-ttu-id="de53f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de53f-118">Application</span></span> | <span data-ttu-id="de53f-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de53f-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de53f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de53f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="de53f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de53f-121">Request headers</span></span>
| <span data-ttu-id="de53f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de53f-122">Header</span></span>       | <span data-ttu-id="de53f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="de53f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de53f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de53f-124">Authorization</span></span>  | <span data-ttu-id="de53f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de53f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="de53f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de53f-127">Content-Type</span></span>  | <span data-ttu-id="de53f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="de53f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de53f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de53f-129">Request body</span></span>
<span data-ttu-id="de53f-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="de53f-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="de53f-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="de53f-131">Parameter</span></span>    | <span data-ttu-id="de53f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="de53f-132">Type</span></span>   |<span data-ttu-id="de53f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="de53f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de53f-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="de53f-134">securityEnabledOnly</span></span>|<span data-ttu-id="de53f-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="de53f-135">Boolean</span></span>|<span data-ttu-id="de53f-p106">**true** (указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь) и **false** (указывает, что должны быть возвращены все группы, в которых состоит пользователь). Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="de53f-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="de53f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="de53f-138">Response</span></span>

<span data-ttu-id="de53f-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию строк в тексте отклика, содержащую идентификаторы групп и ролей каталога, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="de53f-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="de53f-140">Пример</span><span class="sxs-lookup"><span data-stu-id="de53f-140">Example</span></span>
<span data-ttu-id="de53f-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="de53f-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="de53f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="de53f-142">Request</span></span>
<span data-ttu-id="de53f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de53f-143">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="de53f-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="de53f-144">Response</span></span>
<span data-ttu-id="de53f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="de53f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
