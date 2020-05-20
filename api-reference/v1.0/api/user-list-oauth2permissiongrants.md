---
title: Перечисление oauth2PermissionGrants
description: Получение списка объектов oAuth2PermissionGrant, представляющих делегированные разрешения разрешений.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c4fd26ec0c67e4311df06947d83c5408e868c149
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290176"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="11dc1-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="11dc1-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="11dc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11dc1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11dc1-105">Получение списка объектов [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) , которые представляют делегированные разрешения, предоставленные для предоставления клиентскому приложению доступа к API от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="11dc1-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="11dc1-106">Запрос делегированных разрешений, предоставленных пользователю, будет возвращать только делегированные разрешения, предоставленные специально для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="11dc1-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="11dc1-107">Делегированные разрешения, предоставленные от имени всех пользователей в Организации, _не_ включаются в ответ.</span><span class="sxs-lookup"><span data-stu-id="11dc1-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="11dc1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11dc1-108">Permissions</span></span>

<span data-ttu-id="11dc1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11dc1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11dc1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11dc1-111">Permission type</span></span>      | <span data-ttu-id="11dc1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11dc1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11dc1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11dc1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="11dc1-114">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="11dc1-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="11dc1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11dc1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11dc1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11dc1-116">Not supported.</span></span>    |
|<span data-ttu-id="11dc1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11dc1-117">Application</span></span> | <span data-ttu-id="11dc1-118">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="11dc1-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11dc1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11dc1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11dc1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="11dc1-120">Optional query parameters</span></span>

<span data-ttu-id="11dc1-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="11dc1-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11dc1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11dc1-122">Request headers</span></span>

| <span data-ttu-id="11dc1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="11dc1-123">Name</span></span>           | <span data-ttu-id="11dc1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="11dc1-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="11dc1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11dc1-125">Authorization</span></span>  | <span data-ttu-id="11dc1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11dc1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11dc1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11dc1-128">Request body</span></span>

<span data-ttu-id="11dc1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11dc1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11dc1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="11dc1-130">Response</span></span>

<span data-ttu-id="11dc1-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11dc1-131">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11dc1-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="11dc1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11dc1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="11dc1-133">Request</span></span>

<span data-ttu-id="11dc1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11dc1-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/{id}/oauth2PermissionGrants
```

### <a name="response"></a><span data-ttu-id="11dc1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="11dc1-135">Response</span></span>

<span data-ttu-id="11dc1-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11dc1-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="11dc1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11dc1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 253

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
