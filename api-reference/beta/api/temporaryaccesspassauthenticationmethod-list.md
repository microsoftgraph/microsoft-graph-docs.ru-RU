---
title: Список temporaryAccessPassAuthenticationMethods
description: Получите список объектов temporaryAccessPassAuthenticationMethod и их свойств.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 83fe359ac578b316836f9fe624dc949327f26527
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759890"
---
# <a name="list-temporaryaccesspassauthenticationmethods"></a><span data-ttu-id="8de2d-103">Список temporaryAccessPassAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="8de2d-103">List temporaryAccessPassAuthenticationMethods</span></span>
<span data-ttu-id="8de2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8de2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8de2d-105">Извлечение списка временных [объектовAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  и их свойств.</span><span class="sxs-lookup"><span data-stu-id="8de2d-105">Retrieve a list of a user's [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  objects and their properties.</span></span> <span data-ttu-id="8de2d-106">Этот вызов возвращает только один объект, так как для пользователей может быть установлен только один метод временного пропуска доступа.</span><span class="sxs-lookup"><span data-stu-id="8de2d-106">This call will only return a single object as only one Temporary Access Pass method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="8de2d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8de2d-107">Permissions</span></span>
<span data-ttu-id="8de2d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8de2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="8de2d-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="8de2d-110">Permissions acting on self</span></span>

|<span data-ttu-id="8de2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8de2d-111">Permission type</span></span>      | <span data-ttu-id="8de2d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8de2d-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="8de2d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8de2d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8de2d-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8de2d-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="8de2d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8de2d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8de2d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8de2d-116">Not supported.</span></span> |
| <span data-ttu-id="8de2d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8de2d-117">Application</span></span>                            | <span data-ttu-id="8de2d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8de2d-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="8de2d-119">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="8de2d-119">Permissions acting on other users</span></span>

|<span data-ttu-id="8de2d-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8de2d-120">Permission type</span></span>      | <span data-ttu-id="8de2d-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8de2d-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="8de2d-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8de2d-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="8de2d-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8de2d-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="8de2d-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8de2d-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8de2d-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8de2d-125">Not supported.</span></span> |
| <span data-ttu-id="8de2d-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8de2d-126">Application</span></span>                            | <span data-ttu-id="8de2d-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8de2d-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |


<span data-ttu-id="8de2d-128">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="8de2d-128">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="8de2d-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8de2d-129">Global admin</span></span>
* <span data-ttu-id="8de2d-130">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="8de2d-130">Global reader</span></span>
* <span data-ttu-id="8de2d-131">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8de2d-131">Privileged authentication admin</span></span>
* <span data-ttu-id="8de2d-132">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8de2d-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="8de2d-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8de2d-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8de2d-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8de2d-134">Optional query parameters</span></span>
<span data-ttu-id="8de2d-135">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8de2d-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8de2d-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8de2d-136">Request headers</span></span>
|<span data-ttu-id="8de2d-137">Имя</span><span class="sxs-lookup"><span data-stu-id="8de2d-137">Name</span></span>|<span data-ttu-id="8de2d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8de2d-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8de2d-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8de2d-139">Authorization</span></span>|<span data-ttu-id="8de2d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8de2d-p103">Bearer {token}. Required.</span></span>|

## <a name="request"></a><span data-ttu-id="8de2d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8de2d-142">Request</span></span> 
<span data-ttu-id="8de2d-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8de2d-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8de2d-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="8de2d-144">Response</span></span>

<span data-ttu-id="8de2d-145">В случае успеха этот метод возвращает код ответа и коллекцию временных `200 OK` [объектовAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8de2d-145">If successful, this method returns a `200 OK` response code and a collection of [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) objects in the response body.</span></span>  <span data-ttu-id="8de2d-146">Этот вызов возвращает только один объект, так как для пользователей может быть установлен только один **временный ОбъектAccessPassAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="8de2d-146">This call will only return a single object because only one **temporaryAccessPassAuthenticationMethod** can be set on users.</span></span>

## <a name="examples"></a><span data-ttu-id="8de2d-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="8de2d-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8de2d-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8de2d-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8de2d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="8de2d-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/temporaryAccessPassMethods
```
# <a name="c"></a>[<span data-ttu-id="8de2d-150">C#</span><span class="sxs-lookup"><span data-stu-id="8de2d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8de2d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8de2d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8de2d-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8de2d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8de2d-153">Java</span><span class="sxs-lookup"><span data-stu-id="8de2d-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8de2d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="8de2d-154">Response</span></span>
<span data-ttu-id="8de2d-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8de2d-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.temporaryAccessPassAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
      "id": "String",
      "temporaryAccessPass": "String",
      "createdDateTime": "String (timestamp)",
      "startDateTime": "String (timestamp)",
      "lifetimeInMinutes": "Integer",
      "isUsableOnce": "Boolean",
      "isUsable": "Boolean",
      "methodUsabilityReason": "String"
    }
  ]
}
```
