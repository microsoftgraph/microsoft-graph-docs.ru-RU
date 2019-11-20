---
title: 'servicePrincipal: Упдатепассвордсинглесигнонкредентиалс'
description: Обновление учетных данных единого входа с помощью пароля пользователя или группы.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30e629bddd7de3e55b83c43760d5f146c6849a27
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747821"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="3e46a-103">servicePrincipal: Упдатепассвордсинглесигнонкредентиалс</span><span class="sxs-lookup"><span data-stu-id="3e46a-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e46a-104">Обновление учетных данных единого входа с помощью пароля пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="3e46a-104">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e46a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e46a-105">Permissions</span></span>

<span data-ttu-id="3e46a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e46a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e46a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e46a-108">Permission type</span></span>                        | <span data-ttu-id="3e46a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e46a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e46a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e46a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e46a-111">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. AccessAsUser. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3e46a-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3e46a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e46a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e46a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e46a-113">Not supported.</span></span> |
| <span data-ttu-id="3e46a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e46a-114">Application</span></span>                            | <span data-ttu-id="3e46a-115">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3e46a-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="3e46a-116">Пользователи могут самостоятельно создавать учетные данные.</span><span class="sxs-lookup"><span data-stu-id="3e46a-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="3e46a-117">Владельцы и администраторы участников службы могут создавать учетные данные для каждого пользователя или группы: Глобаладминистратор, Аппликатионадминистратор, Клаудаппликатионадминистратор.</span><span class="sxs-lookup"><span data-stu-id="3e46a-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="3e46a-118">Чтобы узнать больше, ознакомьтесь с разделами [роли каталога](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="3e46a-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="3e46a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e46a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="3e46a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e46a-120">Request headers</span></span>

| <span data-ttu-id="3e46a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3e46a-121">Name</span></span>          | <span data-ttu-id="3e46a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3e46a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3e46a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e46a-123">Authorization</span></span> | <span data-ttu-id="3e46a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e46a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e46a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e46a-126">Content-Type</span></span>  | <span data-ttu-id="3e46a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e46a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e46a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e46a-129">Request body</span></span>

<span data-ttu-id="3e46a-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3e46a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e46a-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="3e46a-131">Parameter</span></span>    | <span data-ttu-id="3e46a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3e46a-132">Type</span></span>        | <span data-ttu-id="3e46a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3e46a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e46a-134">id</span><span class="sxs-lookup"><span data-stu-id="3e46a-134">id</span></span>|<span data-ttu-id="3e46a-135">Строка</span><span class="sxs-lookup"><span data-stu-id="3e46a-135">String</span></span>|<span data-ttu-id="3e46a-136">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="3e46a-136">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="3e46a-137">записей</span><span class="sxs-lookup"><span data-stu-id="3e46a-137">credentials</span></span>|<span data-ttu-id="3e46a-138">Коллекция [учетных данных](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="3e46a-138">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="3e46a-139">Список объектов учетных данных, определяющих полный вход.</span><span class="sxs-lookup"><span data-stu-id="3e46a-139">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="3e46a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e46a-140">Response</span></span>

<span data-ttu-id="3e46a-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e46a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e46a-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="3e46a-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e46a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e46a-144">Request</span></span>

<span data-ttu-id="3e46a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e46a-145">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3e46a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e46a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_updatepasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58",
  "credentials": [
    {
      "fieldId": "param_username",
      "value": "myusername",
      "type": "username"
    },
    {
      "fieldId": "param_password",
      "value": "pa$$w0rd",
      "type": "password"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e46a-147">C#</span><span class="sxs-lookup"><span data-stu-id="3e46a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-updatepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e46a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e46a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-updatepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e46a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e46a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-updatepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e46a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e46a-150">Response</span></span>

<span data-ttu-id="3e46a-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3e46a-151">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: updatePasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
