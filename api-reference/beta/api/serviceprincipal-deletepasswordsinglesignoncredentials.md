---
title: 'servicePrincipal: Делетепассвордсинглесигнонкредентиалс'
description: Удаление учетных данных единого входа с помощью пароля пользователя или группы.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72244f521644be4d71ea2aa6e457a2bf61c0742b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453480"
---
# <a name="serviceprincipal-deletepasswordsinglesignoncredentials"></a><span data-ttu-id="65dd9-103">servicePrincipal: Делетепассвордсинглесигнонкредентиалс</span><span class="sxs-lookup"><span data-stu-id="65dd9-103">servicePrincipal: deletePasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="65dd9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="65dd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65dd9-105">Удаление учетных данных единого входа с помощью пароля пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="65dd9-105">Delete single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="65dd9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65dd9-106">Permissions</span></span>

<span data-ttu-id="65dd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65dd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65dd9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65dd9-109">Permission type</span></span>                        | <span data-ttu-id="65dd9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65dd9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="65dd9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65dd9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65dd9-112">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. AccessAsUser. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="65dd9-112">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="65dd9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65dd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65dd9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65dd9-114">Not supported.</span></span> |
| <span data-ttu-id="65dd9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65dd9-115">Application</span></span>                            | <span data-ttu-id="65dd9-116">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="65dd9-116">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="65dd9-117">Пользователи могут самостоятельно создавать учетные данные.</span><span class="sxs-lookup"><span data-stu-id="65dd9-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="65dd9-118">Владельцы и администраторы участников службы могут создавать учетные данные для каждого пользователя или группы: Глобаладминистратор, Аппликатионадминистратор, Клаудаппликатионадминистратор.</span><span class="sxs-lookup"><span data-stu-id="65dd9-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="65dd9-119">Чтобы узнать больше, ознакомьтесь с разделами [роли каталога](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="65dd9-119">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="65dd9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65dd9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="65dd9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65dd9-121">Request headers</span></span>

| <span data-ttu-id="65dd9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="65dd9-122">Name</span></span>          | <span data-ttu-id="65dd9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="65dd9-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="65dd9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65dd9-124">Authorization</span></span> | <span data-ttu-id="65dd9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65dd9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65dd9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65dd9-127">Content-Type</span></span>  | <span data-ttu-id="65dd9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65dd9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65dd9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65dd9-130">Request body</span></span>

<span data-ttu-id="65dd9-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="65dd9-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="65dd9-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="65dd9-132">Parameter</span></span>    | <span data-ttu-id="65dd9-133">Тип</span><span class="sxs-lookup"><span data-stu-id="65dd9-133">Type</span></span>        | <span data-ttu-id="65dd9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="65dd9-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65dd9-135">id</span><span class="sxs-lookup"><span data-stu-id="65dd9-135">id</span></span>|<span data-ttu-id="65dd9-136">String</span><span class="sxs-lookup"><span data-stu-id="65dd9-136">String</span></span>|<span data-ttu-id="65dd9-137">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="65dd9-137">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="65dd9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="65dd9-138">Response</span></span>

<span data-ttu-id="65dd9-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="65dd9-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65dd9-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="65dd9-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65dd9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="65dd9-142">Request</span></span>

<span data-ttu-id="65dd9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65dd9-143">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65dd9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="65dd9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_deletepasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58"
}
```
# <a name="c"></a>[<span data-ttu-id="65dd9-145">C#</span><span class="sxs-lookup"><span data-stu-id="65dd9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-deletepasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65dd9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65dd9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-deletepasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65dd9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65dd9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-deletepasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65dd9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="65dd9-148">Response</span></span>

<span data-ttu-id="65dd9-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="65dd9-149">The following is an example of the response.</span></span>
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
  "description": "servicePrincipal: deletePasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
