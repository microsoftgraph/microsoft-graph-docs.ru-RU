---
title: 'servicePrincipal: Креатепассвордсинглесигнонкредентиалс'
description: Создайте учетные данные единого входа, используя пароль для пользователя или группы.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0df32420eb0431f5eb4f020905ff7eeb3246bb2b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219328"
---
# <a name="serviceprincipal-createpasswordsinglesignoncredentials"></a><span data-ttu-id="0651a-103">servicePrincipal: Креатепассвордсинглесигнонкредентиалс</span><span class="sxs-lookup"><span data-stu-id="0651a-103">servicePrincipal: createPasswordSingleSignOnCredentials</span></span>

<span data-ttu-id="0651a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0651a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0651a-105">Создайте учетные данные единого входа, используя пароль для пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="0651a-105">Create single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0651a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0651a-106">Permissions</span></span>

<span data-ttu-id="0651a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0651a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0651a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0651a-109">Permission type</span></span>                        | <span data-ttu-id="0651a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0651a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0651a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0651a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0651a-112">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. AccessAsUser. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0651a-112">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="0651a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0651a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0651a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0651a-114">Not supported.</span></span> |
| <span data-ttu-id="0651a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0651a-115">Application</span></span>                            | <span data-ttu-id="0651a-116">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0651a-116">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="0651a-117">Пользователи могут самостоятельно создавать учетные данные.</span><span class="sxs-lookup"><span data-stu-id="0651a-117">Users can create credentials for themselves.</span></span> <span data-ttu-id="0651a-118">Владельцы и администраторы участников службы могут создавать учетные данные для каждого пользователя или группы: Глобаладминистратор, Аппликатионадминистратор, Клаудаппликатионадминистратор.</span><span class="sxs-lookup"><span data-stu-id="0651a-118">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="0651a-119">Чтобы узнать больше, ознакомьтесь с разделами [роли каталога](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="0651a-119">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="0651a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0651a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/createPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="0651a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0651a-121">Request headers</span></span>

| <span data-ttu-id="0651a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0651a-122">Name</span></span>          | <span data-ttu-id="0651a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0651a-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0651a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0651a-124">Authorization</span></span> | <span data-ttu-id="0651a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0651a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0651a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0651a-127">Content-Type</span></span>  | <span data-ttu-id="0651a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0651a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0651a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0651a-130">Request body</span></span>

<span data-ttu-id="0651a-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0651a-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0651a-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="0651a-132">Parameter</span></span>    | <span data-ttu-id="0651a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0651a-133">Type</span></span>        | <span data-ttu-id="0651a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0651a-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0651a-135">id</span><span class="sxs-lookup"><span data-stu-id="0651a-135">id</span></span>|<span data-ttu-id="0651a-136">String</span><span class="sxs-lookup"><span data-stu-id="0651a-136">String</span></span>|<span data-ttu-id="0651a-137">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0651a-137">The ID of the user or group this credential set belongs to.</span></span>|
|<span data-ttu-id="0651a-138">записей</span><span class="sxs-lookup"><span data-stu-id="0651a-138">credentials</span></span>|<span data-ttu-id="0651a-139">Коллекция [учетных данных](../resources/credential.md)</span><span class="sxs-lookup"><span data-stu-id="0651a-139">[credential](../resources/credential.md) collection</span></span>|<span data-ttu-id="0651a-140">Список объектов учетных данных, определяющих полный вход.</span><span class="sxs-lookup"><span data-stu-id="0651a-140">A list of credential objects that define the complete sign in flow.</span></span>|

## <a name="response"></a><span data-ttu-id="0651a-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="0651a-141">Response</span></span>

<span data-ttu-id="0651a-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [пассвордсинглесигнонкредентиалсет](../resources/passwordsinglesignoncredentialset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0651a-142">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0651a-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="0651a-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0651a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0651a-144">Request</span></span>

<span data-ttu-id="0651a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0651a-145">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0651a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="0651a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_createpasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/createPasswordSingleSignOnCredentials
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
# <a name="c"></a>[<span data-ttu-id="0651a-147">C#</span><span class="sxs-lookup"><span data-stu-id="0651a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-createpasswordsinglesignoncredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0651a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0651a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-createpasswordsinglesignoncredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0651a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0651a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-createpasswordsinglesignoncredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0651a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="0651a-150">Response</span></span>

<span data-ttu-id="0651a-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0651a-151">The following is an example of the response.</span></span>

> <span data-ttu-id="0651a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0651a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "servicePrincipal: createPasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
