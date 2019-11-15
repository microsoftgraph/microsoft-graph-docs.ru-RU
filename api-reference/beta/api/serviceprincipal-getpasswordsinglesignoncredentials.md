---
title: 'servicePrincipal: Жетпассвордсинглесигнонкредентиалс'
description: Получение списка учетных данных единого входа с помощью пароля пользователя или группы.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ca4c93c944912a0c40ed356a6e6f371e21bb4f0a
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658746"
---
# <a name="serviceprincipal-getpasswordsinglesignoncredentials"></a><span data-ttu-id="0a233-103">servicePrincipal: Жетпассвордсинглесигнонкредентиалс</span><span class="sxs-lookup"><span data-stu-id="0a233-103">servicePrincipal: getPasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a233-104">Получение списка учетных данных единого входа с помощью пароля пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="0a233-104">Get a list of single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a233-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a233-105">Permissions</span></span>

<span data-ttu-id="0a233-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a233-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a233-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a233-108">Permission type</span></span>                        | <span data-ttu-id="0a233-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a233-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a233-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a233-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a233-111">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. AccessAsUser. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0a233-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="0a233-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a233-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a233-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a233-113">Not supported.</span></span> |
| <span data-ttu-id="0a233-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a233-114">Application</span></span>                            | <span data-ttu-id="0a233-115">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0a233-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="0a233-116">Пользователи могут самостоятельно создавать учетные данные.</span><span class="sxs-lookup"><span data-stu-id="0a233-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="0a233-117">Владельцы и администраторы участников службы могут создавать учетные данные для каждого пользователя или группы: Глобаладминистратор, Аппликатионадминистратор, Клаудаппликатионадминистратор.</span><span class="sxs-lookup"><span data-stu-id="0a233-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="0a233-118">Чтобы узнать больше, ознакомьтесь с разделами [роли каталога](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="0a233-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="0a233-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a233-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/getPasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="0a233-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a233-120">Request headers</span></span>

| <span data-ttu-id="0a233-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0a233-121">Name</span></span>          | <span data-ttu-id="0a233-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0a233-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0a233-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a233-123">Authorization</span></span> | <span data-ttu-id="0a233-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a233-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a233-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a233-126">Content-Type</span></span>  | <span data-ttu-id="0a233-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a233-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a233-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a233-129">Request body</span></span>

<span data-ttu-id="0a233-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0a233-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0a233-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="0a233-131">Parameter</span></span>    | <span data-ttu-id="0a233-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0a233-132">Type</span></span>        | <span data-ttu-id="0a233-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0a233-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a233-134">id</span><span class="sxs-lookup"><span data-stu-id="0a233-134">id</span></span>|<span data-ttu-id="0a233-135">String</span><span class="sxs-lookup"><span data-stu-id="0a233-135">String</span></span>|<span data-ttu-id="0a233-136">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0a233-136">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="0a233-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a233-137">Response</span></span>

<span data-ttu-id="0a233-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [пассвордсинглесигнонкредентиалсет](../resources/passwordsinglesignoncredentialset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a233-138">If successful, this method returns a `200 OK` response code and a new [passwordSingleSignOnCredentialSet](../resources/passwordsinglesignoncredentialset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a233-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="0a233-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a233-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a233-140">Request</span></span>

<span data-ttu-id="0a233-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a233-141">The following is an example of a request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a233-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a233-142">Response</span></span>

<span data-ttu-id="0a233-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a233-143">The following is an example of the response.</span></span>

> <span data-ttu-id="0a233-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a233-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
