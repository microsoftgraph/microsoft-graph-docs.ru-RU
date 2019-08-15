---
title: 'Аппликатионтемплате: создание экземпляра'
description: Используйте этот API для создания нового Аппликатионтемплате
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d8ae72372332979c1d6acc3d9d06e8913b454d9e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408196"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="6ea9e-103">Аппликатионтемплате: создание экземпляра</span><span class="sxs-lookup"><span data-stu-id="6ea9e-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ea9e-104">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ea9e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ea9e-105">Permissions</span></span>

<span data-ttu-id="6ea9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ea9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ea9e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ea9e-108">Permission type</span></span>                        | <span data-ttu-id="6ea9e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ea9e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6ea9e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ea9e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ea9e-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ea9e-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="6ea9e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ea9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ea9e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-113">Not supported.</span></span> |
| <span data-ttu-id="6ea9e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ea9e-114">Application</span></span>                            | <span data-ttu-id="6ea9e-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ea9e-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ea9e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ea9e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="6ea9e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ea9e-117">Request headers</span></span>

| <span data-ttu-id="6ea9e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6ea9e-118">Name</span></span>          | <span data-ttu-id="6ea9e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea9e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6ea9e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ea9e-120">Authorization</span></span> | <span data-ttu-id="6ea9e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6ea9e-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ea9e-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ea9e-122">Request body</span></span>

<span data-ttu-id="6ea9e-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6ea9e-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="6ea9e-124">Parameter</span></span>    | <span data-ttu-id="6ea9e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="6ea9e-125">Type</span></span>        | <span data-ttu-id="6ea9e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="6ea9e-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6ea9e-127">displayName</span><span class="sxs-lookup"><span data-stu-id="6ea9e-127">displayName</span></span>|<span data-ttu-id="6ea9e-128">String</span><span class="sxs-lookup"><span data-stu-id="6ea9e-128">String</span></span>|<span data-ttu-id="6ea9e-129">Настраиваемое имя приложения</span><span class="sxs-lookup"><span data-stu-id="6ea9e-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="6ea9e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ea9e-130">Response</span></span>

<span data-ttu-id="6ea9e-131">В случае успешного выполнения этот метод возвращает `201 OK` код отклика и новый объект [аппликатионсервицепринЦипал](../resources/applicationserviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ea9e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ea9e-132">Examples</span></span>

<span data-ttu-id="6ea9e-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6ea9e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ea9e-134">Request</span></span>

<span data-ttu-id="6ea9e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ea9e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea9e-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ea9e-137">C#</span><span class="sxs-lookup"><span data-stu-id="6ea9e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ea9e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ea9e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ea9e-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6ea9e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ea9e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ea9e-140">Response</span></span>

<span data-ttu-id="6ea9e-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="6ea9e-142">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6ea9e-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ea9e-143">All the properties will be returned from an actual call.</span></span>

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
