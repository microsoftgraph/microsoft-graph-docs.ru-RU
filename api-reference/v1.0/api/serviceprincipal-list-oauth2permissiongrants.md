---
title: Перечисление oauth2PermissionGrants
description: Получение списка объектов oAuth2PermissionGrant, представляющих делегированные разрешения разрешений.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 707a8d793f3bbf4cd58f8d68409d698622967c0f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291113"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="24bea-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="24bea-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="24bea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24bea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24bea-105">Получение списка сущностей [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) , представляющих делегированные разрешения, предоставленные субъекту-службе (представляющему клиентское приложение) для доступа к API от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="24bea-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, representing delegated permissions granted to the service principal (representing the client application) to access an API on behalf of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="24bea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24bea-106">Permissions</span></span>

<span data-ttu-id="24bea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24bea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24bea-109">Permission type</span></span>      | <span data-ttu-id="24bea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="24bea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24bea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24bea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="24bea-112">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="24bea-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="24bea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24bea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24bea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24bea-114">Not supported.</span></span>    |
|<span data-ttu-id="24bea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24bea-115">Application</span></span> | <span data-ttu-id="24bea-116">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="24bea-116">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24bea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24bea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24bea-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="24bea-118">Optional query parameters</span></span>

<span data-ttu-id="24bea-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="24bea-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24bea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24bea-120">Request headers</span></span>

| <span data-ttu-id="24bea-121">Имя</span><span class="sxs-lookup"><span data-stu-id="24bea-121">Name</span></span>           | <span data-ttu-id="24bea-122">Описание</span><span class="sxs-lookup"><span data-stu-id="24bea-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="24bea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24bea-123">Authorization</span></span>  | <span data-ttu-id="24bea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24bea-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="24bea-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24bea-126">Request body</span></span>

<span data-ttu-id="24bea-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24bea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24bea-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="24bea-128">Response</span></span>

<span data-ttu-id="24bea-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24bea-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24bea-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="24bea-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24bea-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="24bea-131">Request</span></span>

<span data-ttu-id="24bea-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24bea-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_servicePrincipal_oAuth2PermissionGrants"
}-->

```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/oauth2PermissionGrants
```

### <a name="response"></a><span data-ttu-id="24bea-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="24bea-133">Response</span></span>

<span data-ttu-id="24bea-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24bea-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="24bea-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24bea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
