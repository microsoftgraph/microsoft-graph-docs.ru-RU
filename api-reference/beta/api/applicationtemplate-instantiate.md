---
title: 'Аппликатионтемплате: создание экземпляра'
description: Используйте этот API для создания нового Аппликатионтемплате
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f37cc7351449fc2fadbf259dde16682545ccc235
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441384"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="b9df0-103">Аппликатионтемплате: создание экземпляра</span><span class="sxs-lookup"><span data-stu-id="b9df0-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="b9df0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b9df0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9df0-105">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="b9df0-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9df0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9df0-106">Permissions</span></span>

<span data-ttu-id="b9df0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9df0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9df0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9df0-109">Permission type</span></span>                        | <span data-ttu-id="b9df0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9df0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9df0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9df0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9df0-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9df0-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="b9df0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9df0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9df0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9df0-114">Not supported.</span></span> |
| <span data-ttu-id="b9df0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9df0-115">Application</span></span>                            | <span data-ttu-id="b9df0-116">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9df0-116">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9df0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9df0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="b9df0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9df0-118">Request headers</span></span>

| <span data-ttu-id="b9df0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b9df0-119">Name</span></span>          | <span data-ttu-id="b9df0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b9df0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b9df0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9df0-121">Authorization</span></span> | <span data-ttu-id="b9df0-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b9df0-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9df0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9df0-123">Request body</span></span>

<span data-ttu-id="b9df0-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b9df0-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9df0-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="b9df0-125">Parameter</span></span>    | <span data-ttu-id="b9df0-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b9df0-126">Type</span></span>        | <span data-ttu-id="b9df0-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b9df0-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9df0-128">displayName</span><span class="sxs-lookup"><span data-stu-id="b9df0-128">displayName</span></span>|<span data-ttu-id="b9df0-129">String</span><span class="sxs-lookup"><span data-stu-id="b9df0-129">String</span></span>|<span data-ttu-id="b9df0-130">Настраиваемое имя приложения</span><span class="sxs-lookup"><span data-stu-id="b9df0-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="b9df0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9df0-131">Response</span></span>

<span data-ttu-id="b9df0-132">В случае успешного выполнения этот метод возвращает `201 OK` код отклика и новый объект [аппликатионсервицепринЦипал](../resources/applicationserviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9df0-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9df0-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9df0-133">Examples</span></span>

<span data-ttu-id="b9df0-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b9df0-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b9df0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9df0-135">Request</span></span>

<span data-ttu-id="b9df0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9df0-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9df0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9df0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/beta/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```
# <a name="c"></a>[<span data-ttu-id="b9df0-138">C#</span><span class="sxs-lookup"><span data-stu-id="b9df0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9df0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9df0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9df0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9df0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9df0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9df0-141">Response</span></span>

<span data-ttu-id="b9df0-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9df0-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b9df0-143">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b9df0-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b9df0-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9df0-144">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal": {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
   },
   "application": {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
        "adminConsentDescription": "adminConsentDescription-value",
        "adminConsentDisplayName": "adminConsentDisplayName-value",
        "id": "id-value",
        "isEnabled": true,
        "type": "type-value",
        "userConsentDescription": "userConsentDescription-value",
        "userConsentDisplayName": "userConsentDisplayName-value",
        "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
