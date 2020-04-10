---
title: 'servicePrincipal: Упдатепассвордсинглесигнонкредентиалс'
description: Обновление учетных данных единого входа с помощью пароля пользователя или группы.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ab8a6d256c3f90dbaaa7197f87dec4fd230c73d0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218593"
---
# <a name="serviceprincipal-updatepasswordsinglesignoncredentials"></a><span data-ttu-id="2030d-103">servicePrincipal: Упдатепассвордсинглесигнонкредентиалс</span><span class="sxs-lookup"><span data-stu-id="2030d-103">servicePrincipal: updatePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="2030d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2030d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2030d-105">Обновление учетных данных единого входа с помощью пароля пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="2030d-105">Update single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2030d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2030d-106">Permissions</span></span>

<span data-ttu-id="2030d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2030d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2030d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2030d-109">Permission type</span></span>                        | <span data-ttu-id="2030d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2030d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2030d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2030d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2030d-112">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. AccessAsUser. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2030d-112">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="2030d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2030d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2030d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2030d-114">Not supported.</span></span> |
| <span data-ttu-id="2030d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2030d-115">Application</span></span>                            | <span data-ttu-id="2030d-116">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2030d-116">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="2030d-117">Пользователи могут самостоятельно создавать учетные данные.</span><span class="sxs-lookup"><span data-stu-id="2030d-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="2030d-118">Владельцы и администраторы участников службы могут создавать учетные данные для каждого пользователя или группы: Глобаладминистратор, Аппликатионадминистратор, Клаудаппликатионадминистратор.</span><span class="sxs-lookup"><span data-stu-id="2030d-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="2030d-119">Чтобы узнать больше, ознакомьтесь с разделами [роли каталога](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="2030d-119">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="2030d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2030d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/updatePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="2030d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2030d-121">Request headers</span></span>

| <span data-ttu-id="2030d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2030d-122">Name</span></span>          | <span data-ttu-id="2030d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2030d-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2030d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2030d-124">Authorization</span></span> | <span data-ttu-id="2030d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2030d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2030d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2030d-127">Content-Type</span></span>  | <span data-ttu-id="2030d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2030d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2030d-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2030d-130">Request body</span></span>

<span data-ttu-id="2030d-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2030d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2030d-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="2030d-132">Parameter</span></span>    | <span data-ttu-id="2030d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2030d-133">Type</span></span>        | <span data-ttu-id="2030d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2030d-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2030d-135">id</span><span class="sxs-lookup"><span data-stu-id="2030d-135">id</span></span>|<span data-ttu-id="2030d-136">Строка</span><span class="sxs-lookup"><span data-stu-id="2030d-136">String</span></span>|<span data-ttu-id="2030d-137">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="2030d-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="2030d-138">записей</span><span class="sxs-lookup"><span data-stu-id="2030d-138">credentials</span></span>|<span data-ttu-id="2030d-139">Коллекция [учетных данных](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="2030d-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="2030d-140">Список объектов учетных данных, определяющих полный вход.</span><span class="sxs-lookup"><span data-stu-id="2030d-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="2030d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2030d-141">Response</span></span>

<span data-ttu-id="2030d-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2030d-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2030d-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="2030d-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2030d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="2030d-145">Request</span></span>

<span data-ttu-id="2030d-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2030d-146">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2030d-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="2030d-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2030d-148">C#</span><span class="sxs-lookup"><span data-stu-id="2030d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-updatepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2030d-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2030d-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-updatepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2030d-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2030d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-updatepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2030d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2030d-151">Response</span></span>

<span data-ttu-id="2030d-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2030d-152">The following is an example of the response.</span></span>
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
