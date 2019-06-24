---
title: 'Аппликатионтемплате: создание экземпляра'
description: Используйте этот API для создания нового Аппликатионтемплате
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d3874f7e015816dbc76ce99fa1fc26f65727ad97
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147932"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="d0b63-103">Аппликатионтемплате: создание экземпляра</span><span class="sxs-lookup"><span data-stu-id="d0b63-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0b63-104">Добавьте экземпляр приложения из коллекции приложений Azure AD в ваш каталог.</span><span class="sxs-lookup"><span data-stu-id="d0b63-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0b63-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b63-105">Permissions</span></span>

<span data-ttu-id="d0b63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0b63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0b63-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b63-108">Permission type</span></span>                        | <span data-ttu-id="d0b63-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0b63-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0b63-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0b63-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0b63-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0b63-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="d0b63-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0b63-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0b63-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b63-113">Not supported.</span></span> |
| <span data-ttu-id="d0b63-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0b63-114">Application</span></span>                            | <span data-ttu-id="d0b63-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0b63-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0b63-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0b63-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="d0b63-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0b63-117">Request headers</span></span>

| <span data-ttu-id="d0b63-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d0b63-118">Name</span></span>          | <span data-ttu-id="d0b63-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d0b63-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d0b63-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0b63-120">Authorization</span></span> | <span data-ttu-id="d0b63-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d0b63-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0b63-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0b63-122">Request body</span></span>

<span data-ttu-id="d0b63-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d0b63-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d0b63-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="d0b63-124">Parameter</span></span>    | <span data-ttu-id="d0b63-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d0b63-125">Type</span></span>        | <span data-ttu-id="d0b63-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d0b63-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0b63-127">displayName</span><span class="sxs-lookup"><span data-stu-id="d0b63-127">displayName</span></span>|<span data-ttu-id="d0b63-128">String</span><span class="sxs-lookup"><span data-stu-id="d0b63-128">String</span></span>|<span data-ttu-id="d0b63-129">Настраиваемое имя приложения</span><span class="sxs-lookup"><span data-stu-id="d0b63-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="d0b63-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b63-130">Response</span></span>

<span data-ttu-id="d0b63-131">В случае успешного выполнения этот метод возвращает `201 OK` код отклика и новый объект [аппликатионсервицепринЦипал](../resources/applicationserviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0b63-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d0b63-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="d0b63-132">Examples</span></span>

<span data-ttu-id="d0b63-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d0b63-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d0b63-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0b63-134">Request</span></span>

<span data-ttu-id="d0b63-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0b63-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0b63-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b63-136">Response</span></span>

<span data-ttu-id="d0b63-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d0b63-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d0b63-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0b63-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d0b63-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0b63-139">All the properties will be returned from an actual call.</span></span>

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
