---
title: 'servicePrincipal: Делетепассвордсинглесигнонкредентиалс'
description: Удаление учетных данных единого входа с помощью пароля пользователя или группы.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b39bf30f4a6a943a21db012d0201812681dd9ee
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658823"
---
# <a name="serviceprincipal-deletepasswordsinglesignoncredentials"></a><span data-ttu-id="2ee37-103">servicePrincipal: Делетепассвордсинглесигнонкредентиалс</span><span class="sxs-lookup"><span data-stu-id="2ee37-103">servicePrincipal: deletePasswordSingleSignOnCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ee37-104">Удаление учетных данных единого входа с помощью пароля пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="2ee37-104">Delete single sign-on credentials using a password for a user or group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ee37-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ee37-105">Permissions</span></span>

<span data-ttu-id="2ee37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ee37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ee37-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ee37-108">Permission type</span></span>                        | <span data-ttu-id="2ee37-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ee37-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ee37-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ee37-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ee37-111">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. AccessAsUser. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2ee37-111">Application.ReadWrite.All (also needs Directory.Read.All), Directory.AccessAsUser.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="2ee37-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ee37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ee37-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ee37-113">Not supported.</span></span> |
| <span data-ttu-id="2ee37-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ee37-114">Application</span></span>                            | <span data-ttu-id="2ee37-115">Application. ReadWrite. All (также требуются Directory. Read. ALL), Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2ee37-115">Application.ReadWrite.All (also needs Directory.Read.All), Directory.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="2ee37-116">Пользователи могут самостоятельно создавать учетные данные.</span><span class="sxs-lookup"><span data-stu-id="2ee37-116">Users can create credentials for themselves.</span></span> <span data-ttu-id="2ee37-117">Владельцы и администраторы участников службы могут создавать учетные данные для каждого пользователя или группы: Глобаладминистратор, Аппликатионадминистратор, Клаудаппликатионадминистратор.</span><span class="sxs-lookup"><span data-stu-id="2ee37-117">Service principal owners and admins with the following roles can create credentials for any user or group: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator.</span></span> <span data-ttu-id="2ee37-118">Чтобы узнать больше, ознакомьтесь с разделами [роли каталога](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span><span class="sxs-lookup"><span data-stu-id="2ee37-118">To learn more, see [Directory roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>

## <a name="http-request"></a><span data-ttu-id="2ee37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ee37-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a><span data-ttu-id="2ee37-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ee37-120">Request headers</span></span>

| <span data-ttu-id="2ee37-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2ee37-121">Name</span></span>          | <span data-ttu-id="2ee37-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2ee37-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2ee37-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ee37-123">Authorization</span></span> | <span data-ttu-id="2ee37-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ee37-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ee37-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ee37-126">Content-Type</span></span>  | <span data-ttu-id="2ee37-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ee37-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ee37-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ee37-129">Request body</span></span>

<span data-ttu-id="2ee37-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2ee37-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2ee37-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="2ee37-131">Parameter</span></span>    | <span data-ttu-id="2ee37-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2ee37-132">Type</span></span>        | <span data-ttu-id="2ee37-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2ee37-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ee37-134">id</span><span class="sxs-lookup"><span data-stu-id="2ee37-134">id</span></span>|<span data-ttu-id="2ee37-135">String</span><span class="sxs-lookup"><span data-stu-id="2ee37-135">String</span></span>|<span data-ttu-id="2ee37-136">Идентификатор пользователя или группы, к которой принадлежит этот набор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="2ee37-136">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="response"></a><span data-ttu-id="2ee37-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ee37-137">Response</span></span>

<span data-ttu-id="2ee37-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ee37-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ee37-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ee37-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ee37-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ee37-141">Request</span></span>

<span data-ttu-id="2ee37-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ee37-142">The following is an example of a request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2ee37-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ee37-143">Response</span></span>

<span data-ttu-id="2ee37-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ee37-144">The following is an example of the response.</span></span>
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
