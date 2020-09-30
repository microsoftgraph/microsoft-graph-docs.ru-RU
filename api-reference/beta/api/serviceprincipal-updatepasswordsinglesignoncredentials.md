---
title: 'servicePrincipal: Упдатепассвордсинглесигнонкредентиалс'
description: Обновление учетных данных единого входа с помощью пароля пользователя или группы.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92e276bfc8b87b0d5d372330996a22af878c024b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314309"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="00204-103">servicePrincipal: Упдатепассвордсинглесигнонкредентиалс</span><span class="sxs-lookup"><span data-stu-id="00204-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="00204-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00204-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00204-105">Обновление учетных данных единого входа с помощью пароля пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="00204-105">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="00204-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00204-106">Permissions</span></span>

<span data-ttu-id="00204-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00204-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00204-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00204-109">Permission type</span></span>                        | <span data-ttu-id="00204-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00204-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="00204-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00204-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="00204-112">Application. ReadWrite. ALL и Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="00204-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="00204-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00204-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00204-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00204-114">Not supported.</span></span> |
| <span data-ttu-id="00204-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00204-115">Application</span></span>                            | <span data-ttu-id="00204-116">Application. ReadWrite. ALL и Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="00204-116">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="00204-117">Пользователи могут самостоятельно создавать учетные данные.</span><span class="sxs-lookup"><span data-stu-id="00204-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="00204-118">Владельцы и администраторы участников службы могут создавать учетные данные для каждого пользователя или группы: Глобаладминистратор, Аппликатионадминистратор, Клаудаппликатионадминистратор.</span><span class="sxs-lookup"><span data-stu-id="00204-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="00204-119">Чтобы узнать больше, ознакомьтесь с разделами [роли каталога](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="00204-119">To learn more, see [Directory roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="00204-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00204-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="00204-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00204-121">Request headers</span></span>

| <span data-ttu-id="00204-122">Имя</span><span class="sxs-lookup"><span data-stu-id="00204-122">Name</span></span>          | <span data-ttu-id="00204-123">Описание</span><span class="sxs-lookup"><span data-stu-id="00204-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="00204-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00204-124">Authorization</span></span> | <span data-ttu-id="00204-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00204-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00204-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00204-127">Content-Type</span></span>  | <span data-ttu-id="00204-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00204-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00204-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00204-130">Request body</span></span>

<span data-ttu-id="00204-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="00204-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="00204-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="00204-132">Parameter</span></span>    | <span data-ttu-id="00204-133">Тип</span><span class="sxs-lookup"><span data-stu-id="00204-133">Type</span></span>        | <span data-ttu-id="00204-134">Описание</span><span class="sxs-lookup"><span data-stu-id="00204-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="00204-135">id</span><span class="sxs-lookup"><span data-stu-id="00204-135">id</span></span>|<span data-ttu-id="00204-136">String</span><span class="sxs-lookup"><span data-stu-id="00204-136">String</span></span>|<span data-ttu-id="00204-137">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="00204-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="00204-138">записей</span><span class="sxs-lookup"><span data-stu-id="00204-138">credentials</span></span>|<span data-ttu-id="00204-139">Коллекция [учетных данных](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="00204-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="00204-140">Список объектов учетных данных, определяющих полный вход.</span><span class="sxs-lookup"><span data-stu-id="00204-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="00204-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="00204-141">Response</span></span>

<span data-ttu-id="00204-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="00204-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00204-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="00204-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00204-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="00204-145">Request</span></span>

<span data-ttu-id="00204-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00204-146">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00204-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="00204-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="00204-148">C#</span><span class="sxs-lookup"><span data-stu-id="00204-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-updatepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00204-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00204-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-updatepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00204-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00204-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-updatepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="00204-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="00204-151">Response</span></span>

<span data-ttu-id="00204-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="00204-152">The following is an example of the response.</span></span>
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