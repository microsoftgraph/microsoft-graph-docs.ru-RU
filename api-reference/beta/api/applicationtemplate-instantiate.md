---
title: 'Аппликатионтемплате: создание экземпляра'
description: Используйте этот API для создания нового Аппликатионтемплате
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b44292e2d4f9fd23ba5a1e71c074750a5d507ad2
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372448"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="27d58-103">Аппликатионтемплате: создание экземпляра</span><span class="sxs-lookup"><span data-stu-id="27d58-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="27d58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27d58-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27d58-105">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="27d58-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="27d58-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27d58-106">Permissions</span></span>

<span data-ttu-id="27d58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27d58-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27d58-109">Permission type</span></span>                        | <span data-ttu-id="27d58-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27d58-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27d58-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27d58-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="27d58-112">Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="27d58-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="27d58-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27d58-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27d58-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27d58-114">Not supported.</span></span> |
| <span data-ttu-id="27d58-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="27d58-115">Application</span></span>                            | <span data-ttu-id="27d58-116">Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="27d58-116">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27d58-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27d58-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="27d58-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27d58-118">Request headers</span></span>

| <span data-ttu-id="27d58-119">Имя</span><span class="sxs-lookup"><span data-stu-id="27d58-119">Name</span></span>          | <span data-ttu-id="27d58-120">Описание</span><span class="sxs-lookup"><span data-stu-id="27d58-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="27d58-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27d58-121">Authorization</span></span> | <span data-ttu-id="27d58-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="27d58-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="27d58-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27d58-123">Request body</span></span>

<span data-ttu-id="27d58-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="27d58-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="27d58-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="27d58-125">Parameter</span></span>    | <span data-ttu-id="27d58-126">Тип</span><span class="sxs-lookup"><span data-stu-id="27d58-126">Type</span></span>        | <span data-ttu-id="27d58-127">Описание</span><span class="sxs-lookup"><span data-stu-id="27d58-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27d58-128">displayName</span><span class="sxs-lookup"><span data-stu-id="27d58-128">displayName</span></span>|<span data-ttu-id="27d58-129">String</span><span class="sxs-lookup"><span data-stu-id="27d58-129">String</span></span>|<span data-ttu-id="27d58-130">Настраиваемое имя приложения</span><span class="sxs-lookup"><span data-stu-id="27d58-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="27d58-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="27d58-131">Response</span></span>

<span data-ttu-id="27d58-132">В случае успешного выполнения этот метод возвращает `201 OK` код отклика и новый объект [аппликатионсервицепринЦипал](../resources/applicationserviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27d58-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27d58-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="27d58-133">Examples</span></span>

<span data-ttu-id="27d58-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="27d58-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="27d58-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="27d58-135">Request</span></span>

<span data-ttu-id="27d58-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27d58-136">The following is an example of the request.</span></span>

> [!NOTE] 
> <span data-ttu-id="27d58-137">Вы можете использовать этот API для создания экземпляров [приложений, не относящихся к коллекции](/azure/active-directory/manage-apps/add-non-gallery-app).</span><span class="sxs-lookup"><span data-stu-id="27d58-137">You can use this API to instantiate [non-gallery apps](/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="27d58-138">Используйте следующий идентификатор для **аппликатионтемплате**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="27d58-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

# <a name="http"></a>[<span data-ttu-id="27d58-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="27d58-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="27d58-140">C#</span><span class="sxs-lookup"><span data-stu-id="27d58-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27d58-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27d58-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27d58-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27d58-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27d58-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="27d58-143">Response</span></span>

<span data-ttu-id="27d58-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27d58-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="27d58-145">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="27d58-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="27d58-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27d58-146">All the properties will be returned from an actual call.</span></span>

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
