---
title: 'servicePrincipal: getPasswordSingleSignOnCredentials'
description: Получите список учетных данных единого входа с помощью пароля для пользователя или группы.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e0c98822c24dd9e8775fd3340f96fccacde149a1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134423"
---
# <a name="serviceprincipal-getpasswordsinglesignoncredentials"></a><span data-ttu-id="f7143-103">servicePrincipal: getPasswordSingleSignOnCredentials</span><span class="sxs-lookup"><span data-stu-id="f7143-103">servicePrincipal: getPasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="f7143-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7143-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7143-105">Получите список учетных данных единого входа с помощью пароля для пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="f7143-105">Get a list of single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7143-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7143-106">Permissions</span></span>

<span data-ttu-id="f7143-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7143-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7143-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7143-109">Permission type</span></span>                        | <span data-ttu-id="f7143-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7143-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7143-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7143-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7143-112">Application.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7143-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f7143-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7143-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7143-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7143-114">Not supported.</span></span> |
| <span data-ttu-id="f7143-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7143-115">Application</span></span>                            | <span data-ttu-id="f7143-116">Application.ReadWrite.OwnedBy и Directory.Read.All, Application.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7143-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="f7143-117">Пользователи могут создавать учетные данные для себя.</span><span class="sxs-lookup"><span data-stu-id="f7143-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="f7143-118">Владельцы и администраторы, в которых есть следующие роли, могут создавать учетные данные для любого пользователя или группы: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span><span class="sxs-lookup"><span data-stu-id="f7143-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="f7143-119">Дополнительные узнать см. в [ролях каталога.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="f7143-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="f7143-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7143-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/getPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="f7143-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7143-121">Request headers</span></span>

| <span data-ttu-id="f7143-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f7143-122">Name</span></span>          | <span data-ttu-id="f7143-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f7143-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f7143-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7143-124">Authorization</span></span> | <span data-ttu-id="f7143-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7143-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7143-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7143-127">Content-Type</span></span>  | <span data-ttu-id="f7143-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7143-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7143-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7143-130">Request body</span></span>

<span data-ttu-id="f7143-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f7143-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7143-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7143-132">Parameter</span></span>    | <span data-ttu-id="f7143-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f7143-133">Type</span></span>        | <span data-ttu-id="f7143-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f7143-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7143-135">id</span><span class="sxs-lookup"><span data-stu-id="f7143-135">id</span></span>|<span data-ttu-id="f7143-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f7143-136">String</span></span>|<span data-ttu-id="f7143-137">ИД пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="f7143-137">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="f7143-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7143-138">Response</span></span>

<span data-ttu-id="f7143-139">В случае успеха этот метод возвращает код отклика и новый объект `200 OK` [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7143-139">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7143-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7143-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7143-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7143-141">Request</span></span>

<span data-ttu-id="f7143-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7143-142">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7143-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7143-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getpasswordsinglesignoncredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getPasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58"
}
```
# <a name="c"></a>[<span data-ttu-id="f7143-144">C#</span><span class="sxs-lookup"><span data-stu-id="f7143-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getpasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7143-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7143-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getpasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7143-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7143-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getpasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7143-147">Java</span><span class="sxs-lookup"><span data-stu-id="f7143-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-getpasswordsinglesignoncredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7143-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7143-148">Response</span></span>

<span data-ttu-id="f7143-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7143-149">The following is an example of the response.</span></span>

> <span data-ttu-id="f7143-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7143-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet"
} -->
```http
HTTP/1.1 200 OK
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
      "value": null,
      "type": "password"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: getPasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
