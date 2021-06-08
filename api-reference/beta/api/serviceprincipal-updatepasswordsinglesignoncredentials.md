---
title: 'servicePrincipal: updatePasswordSingleSignOnCredentials'
description: Обновление учетных данных с одним входом с помощью пароля для пользователя или группы.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b178bba8f14dc0359baea9c2178eef2cffdf14ce
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786116"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="2a442-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="2a442-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="2a442-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a442-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a442-105">Обновление учетных данных с одним входом с помощью пароля для пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="2a442-105">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a442-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a442-106">Permissions</span></span>

<span data-ttu-id="2a442-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a442-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a442-109">Permission type</span></span>                        | <span data-ttu-id="2a442-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a442-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a442-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a442-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a442-112">Application.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a442-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2a442-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a442-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a442-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a442-114">Not supported.</span></span> |
| <span data-ttu-id="2a442-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a442-115">Application</span></span>                            | <span data-ttu-id="2a442-116">Application.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a442-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="2a442-117">Пользователи могут создавать учетные данные для себя.</span><span class="sxs-lookup"><span data-stu-id="2a442-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="2a442-118">Владельцы и администраторы служб со следующими ролями могут создавать учетные данные для любого пользователя или группы: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="2a442-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="2a442-119">Дополнительные дополнительные функции см. в [каталоге ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="2a442-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="2a442-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a442-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="2a442-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a442-121">Request headers</span></span>

| <span data-ttu-id="2a442-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2a442-122">Name</span></span>          | <span data-ttu-id="2a442-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2a442-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2a442-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a442-124">Authorization</span></span> | <span data-ttu-id="2a442-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a442-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a442-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a442-127">Content-Type</span></span>  | <span data-ttu-id="2a442-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a442-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a442-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a442-130">Request body</span></span>

<span data-ttu-id="2a442-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2a442-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2a442-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="2a442-132">Parameter</span></span>    | <span data-ttu-id="2a442-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2a442-133">Type</span></span>        | <span data-ttu-id="2a442-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2a442-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a442-135">id</span><span class="sxs-lookup"><span data-stu-id="2a442-135">id</span></span>|<span data-ttu-id="2a442-136">String</span><span class="sxs-lookup"><span data-stu-id="2a442-136">String</span></span>|<span data-ttu-id="2a442-137">ID пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="2a442-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="2a442-138">учетные данные</span><span class="sxs-lookup"><span data-stu-id="2a442-138">credentials</span></span>|<span data-ttu-id="2a442-139">[коллекция учетных](../resources/credential.md) данных</span><span class="sxs-lookup"><span data-stu-id="2a442-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="2a442-140">Список объектов учетных данных, которые определяют полный вход в потоке.</span><span class="sxs-lookup"><span data-stu-id="2a442-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="2a442-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a442-141">Response</span></span>

<span data-ttu-id="2a442-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a442-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a442-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a442-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a442-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a442-145">Request</span></span>

<span data-ttu-id="2a442-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a442-146">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a442-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a442-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2a442-148">C#</span><span class="sxs-lookup"><span data-stu-id="2a442-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-updatepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a442-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a442-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-updatepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a442-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a442-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-updatepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a442-151">Java</span><span class="sxs-lookup"><span data-stu-id="2a442-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-updatepasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a442-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a442-152">Response</span></span>

<span data-ttu-id="2a442-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a442-153">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
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
