---
title: 'Аппликатионтемплате: создание экземпляра'
description: Используйте этот API для создания нового Аппликатионтемплате
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64d754b0053cd63711f4c0a1ef35d8429be84883
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856704"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="672b8-103">Аппликатионтемплате: создание экземпляра</span><span class="sxs-lookup"><span data-stu-id="672b8-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="672b8-104">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="672b8-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="672b8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="672b8-105">Permissions</span></span>

<span data-ttu-id="672b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="672b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="672b8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="672b8-108">Permission type</span></span>                        | <span data-ttu-id="672b8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="672b8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="672b8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="672b8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="672b8-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="672b8-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="672b8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="672b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="672b8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="672b8-113">Not supported.</span></span> |
| <span data-ttu-id="672b8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="672b8-114">Application</span></span>                            | <span data-ttu-id="672b8-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="672b8-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="672b8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="672b8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="672b8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="672b8-117">Request headers</span></span>

| <span data-ttu-id="672b8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="672b8-118">Name</span></span>          | <span data-ttu-id="672b8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="672b8-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="672b8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="672b8-120">Authorization</span></span> | <span data-ttu-id="672b8-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="672b8-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="672b8-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="672b8-122">Request body</span></span>

<span data-ttu-id="672b8-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="672b8-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="672b8-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="672b8-124">Parameter</span></span>    | <span data-ttu-id="672b8-125">Тип</span><span class="sxs-lookup"><span data-stu-id="672b8-125">Type</span></span>        | <span data-ttu-id="672b8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="672b8-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="672b8-127">displayName</span><span class="sxs-lookup"><span data-stu-id="672b8-127">displayName</span></span>|<span data-ttu-id="672b8-128">String</span><span class="sxs-lookup"><span data-stu-id="672b8-128">String</span></span>|<span data-ttu-id="672b8-129">Настраиваемое имя приложения</span><span class="sxs-lookup"><span data-stu-id="672b8-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="672b8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="672b8-130">Response</span></span>

<span data-ttu-id="672b8-131">В случае успешного выполнения этот метод возвращает `201 OK` код отклика и новый объект [аппликатионсервицепринЦипал](../resources/applicationserviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="672b8-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="672b8-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="672b8-132">Examples</span></span>

<span data-ttu-id="672b8-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="672b8-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="672b8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="672b8-134">Request</span></span>

<span data-ttu-id="672b8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="672b8-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="672b8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="672b8-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="672b8-137">C#</span><span class="sxs-lookup"><span data-stu-id="672b8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="672b8-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="672b8-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="672b8-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="672b8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="672b8-140">Java</span><span class="sxs-lookup"><span data-stu-id="672b8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="672b8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="672b8-141">Response</span></span>

<span data-ttu-id="672b8-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="672b8-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="672b8-143">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="672b8-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="672b8-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="672b8-144">All the properties will be returned from an actual call.</span></span>

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
