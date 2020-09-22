---
title: 'Аппликатионтемплате: создание экземпляра'
description: Используйте этот API для создания нового Аппликатионтемплате
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a06ace04fd87b91e56834fe874c8f6de141d7020
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996665"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="c0f54-103">Аппликатионтемплате: создание экземпляра</span><span class="sxs-lookup"><span data-stu-id="c0f54-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="c0f54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0f54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f54-105">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="c0f54-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0f54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0f54-106">Permissions</span></span>

<span data-ttu-id="c0f54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0f54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0f54-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0f54-109">Permission type</span></span>                        | <span data-ttu-id="c0f54-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0f54-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0f54-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0f54-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0f54-112">Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c0f54-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c0f54-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0f54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0f54-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0f54-114">Not supported.</span></span> |
| <span data-ttu-id="c0f54-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0f54-115">Application</span></span>                            | <span data-ttu-id="c0f54-116">Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c0f54-116">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0f54-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0f54-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="c0f54-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0f54-118">Request headers</span></span>

| <span data-ttu-id="c0f54-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c0f54-119">Name</span></span>          | <span data-ttu-id="c0f54-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0f54-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c0f54-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0f54-121">Authorization</span></span> | <span data-ttu-id="c0f54-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c0f54-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0f54-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0f54-123">Request body</span></span>

<span data-ttu-id="c0f54-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c0f54-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c0f54-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="c0f54-125">Parameter</span></span>    | <span data-ttu-id="c0f54-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c0f54-126">Type</span></span>        | <span data-ttu-id="c0f54-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c0f54-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0f54-128">displayName</span><span class="sxs-lookup"><span data-stu-id="c0f54-128">displayName</span></span>|<span data-ttu-id="c0f54-129">String</span><span class="sxs-lookup"><span data-stu-id="c0f54-129">String</span></span>|<span data-ttu-id="c0f54-130">Настраиваемое имя приложения</span><span class="sxs-lookup"><span data-stu-id="c0f54-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="c0f54-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0f54-131">Response</span></span>

<span data-ttu-id="c0f54-132">В случае успешного выполнения этот метод возвращает `201 OK` код отклика и новый объект [аппликатионсервицепринЦипал](../resources/applicationserviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0f54-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0f54-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0f54-133">Examples</span></span>

<span data-ttu-id="c0f54-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c0f54-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c0f54-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0f54-135">Request</span></span>

<span data-ttu-id="c0f54-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0f54-136">The following is an example of the request.</span></span>

> [!NOTE] 
> <span data-ttu-id="c0f54-137">Вы можете использовать этот API для создания экземпляров [приложений, не относящихся к коллекции](https://docs.microsoft.com/azure/active-directory/manage-apps/add-non-gallery-app).</span><span class="sxs-lookup"><span data-stu-id="c0f54-137">You can use this API to instantiate [non-gallery apps](https://docs.microsoft.com/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="c0f54-138">Используйте следующий идентификатор для **аппликатионтемплате**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="c0f54-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0f54-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0f54-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c0f54-140">C#</span><span class="sxs-lookup"><span data-stu-id="c0f54-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0f54-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0f54-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0f54-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0f54-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0f54-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0f54-143">Response</span></span>

<span data-ttu-id="c0f54-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0f54-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c0f54-145">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0f54-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c0f54-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0f54-146">All the properties will be returned from an actual call.</span></span>

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


