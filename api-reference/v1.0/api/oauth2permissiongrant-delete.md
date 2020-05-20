---
title: Удаление oAuth2PermissionGrant
description: Удаление объекта oAuth2PermissionGrant, представляющего делегированное предоставление разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bc36f62d1bb0568fc24b48061e427c404f16e43c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288928"
---
# <a name="delete-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="a89a0-103">Удаление делегированного предоставления разрешений (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="a89a0-103">Delete a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="a89a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a89a0-105">Удаление [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span><span class="sxs-lookup"><span data-stu-id="a89a0-105">Delete an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).</span></span>

<span data-ttu-id="a89a0-106">При удалении делегированного разрешения предоставленный им доступ отзывается.</span><span class="sxs-lookup"><span data-stu-id="a89a0-106">When a delegated permission grant is deleted, the access it granted is revoked.</span></span> <span data-ttu-id="a89a0-107">Существующие маркеры доступа продолжат действовать в течение всего времени существования, но новые маркеры доступа не будут предоставлены делегированным разрешениям, определенным в удаленном **oAuth2PermissionGrant**.</span><span class="sxs-lookup"><span data-stu-id="a89a0-107">Existing access tokens will continue to be valid for their lifetime, but new access tokens will not be granted for the delegated permissions identified in the deleted **oAuth2PermissionGrant**.</span></span>

> [!NOTE]
> <span data-ttu-id="a89a0-108">Можно предоставить два делегированных разрешения на авторизацию приложения, действующего от имени пользователя при вызове API.</span><span class="sxs-lookup"><span data-stu-id="a89a0-108">There may be two delegated permission grants authorizing an application to act on behalf of a user when calling an API.</span></span> <span data-ttu-id="a89a0-109">Это может произойти, когда пользователь отправляет приложение по собственному имени (создавая **oAuth2PermissionGrant** с *участником* **консенттипе** , определяя пользователя), а затем администратор предоставляет согласие администратора на уровне клиента от имени всех пользователей (создание второго **oAuth2PermissionGrant** с **консенттипе** *аллпринЦипалс*).</span><span class="sxs-lookup"><span data-stu-id="a89a0-109">This can happen when a user consents for the application on their own behalf (creating an **oAuth2PermissionGrant** with **consentType** *Principal*, identifying the user) and then an administrator grants tenant-wide admin consent on behalf of all users (creating a second **oAuth2PermissionGrant** with **consentType** of *AllPrincipals*).</span></span>

## <a name="permissions"></a><span data-ttu-id="a89a0-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a89a0-110">Permissions</span></span>

<span data-ttu-id="a89a0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89a0-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a89a0-113">Permission type</span></span>      | <span data-ttu-id="a89a0-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a89a0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a89a0-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a89a0-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a89a0-116">Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="a89a0-116">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a89a0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a89a0-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a89a0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89a0-118">Not supported.</span></span>    |
|<span data-ttu-id="a89a0-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a89a0-119">Application</span></span> | <span data-ttu-id="a89a0-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89a0-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a89a0-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a89a0-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /oAuth2Permissiongrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a89a0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a89a0-122">Request headers</span></span>

| <span data-ttu-id="a89a0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a89a0-123">Name</span></span>       | <span data-ttu-id="a89a0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a89a0-124">Type</span></span> | <span data-ttu-id="a89a0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a89a0-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a89a0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a89a0-126">Authorization</span></span>  | <span data-ttu-id="a89a0-127">string</span><span class="sxs-lookup"><span data-stu-id="a89a0-127">string</span></span>  | <span data-ttu-id="a89a0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a89a0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a89a0-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a89a0-130">Request body</span></span>

<span data-ttu-id="a89a0-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a89a0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a89a0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89a0-132">Response</span></span>

<span data-ttu-id="a89a0-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a89a0-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a89a0-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a89a0-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="a89a0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a89a0-136">Request</span></span>

<span data-ttu-id="a89a0-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a89a0-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a89a0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a89a0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2PermissionGrant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
```

### <a name="response"></a><span data-ttu-id="a89a0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89a0-139">Response</span></span>

<span data-ttu-id="a89a0-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a89a0-140">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
