---
title: Создание приложения
description: Используйте этот интерфейс API для создания нового приложения.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8cde90f31f7583d24361f6935701a91f69d7cfde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941473"
---
# <a name="create-application"></a><span data-ttu-id="03376-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="03376-103">Create Application</span></span>

> <span data-ttu-id="03376-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03376-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03376-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03376-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03376-106">Используйте этот интерфейс API для создания нового приложения.</span><span class="sxs-lookup"><span data-stu-id="03376-106">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="03376-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03376-107">Permissions</span></span>
<span data-ttu-id="03376-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03376-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="03376-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03376-110">Permission type</span></span>      | <span data-ttu-id="03376-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03376-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03376-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03376-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03376-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03376-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03376-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03376-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03376-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03376-115">Not supported.</span></span>    |
|<span data-ttu-id="03376-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03376-116">Application</span></span> | <span data-ttu-id="03376-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03376-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03376-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03376-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="03376-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03376-119">Request headers</span></span>
| <span data-ttu-id="03376-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03376-120">Name</span></span>       | <span data-ttu-id="03376-121">Тип</span><span class="sxs-lookup"><span data-stu-id="03376-121">Type</span></span> | <span data-ttu-id="03376-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03376-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03376-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03376-123">Authorization</span></span>  | <span data-ttu-id="03376-124">строка</span><span class="sxs-lookup"><span data-stu-id="03376-124">string</span></span>  | <span data-ttu-id="03376-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03376-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03376-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03376-127">Request body</span></span>
<span data-ttu-id="03376-128">В тексте запроса укажите представление JSON объекта [приложения](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="03376-128">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="03376-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="03376-129">Response</span></span>

<span data-ttu-id="03376-130">Успешно завершена, этот метод возвращает `201 Created` объект ответа кодов и [приложений](../resources/application.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="03376-130">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03376-131">Пример</span><span class="sxs-lookup"><span data-stu-id="03376-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03376-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="03376-132">Request</span></span>
<span data-ttu-id="03376-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03376-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "allowPublicClient": true,
  "displayName": "Display name"
}
```
<span data-ttu-id="03376-134">В тексте запроса укажите представление JSON объекта [приложения](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="03376-134">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="03376-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="03376-135">Response</span></span>
<span data-ttu-id="03376-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="03376-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
    "id": "b5b2920e-a47c-43b7-91ef-25ae96fddddd",
    "deletedDateTime": null,
    "api": {
        "acceptedAccessTokenVersion": 2,
        "publishedPermissionScopes": []
    },
    "allowPublicClient": true,
    "applicationAliases": [],
    "appRoles": [],
    "createdDateTime": "2017-05-25T16:33:04.3646617Z",
    "installedClients": {
        "redirectUrls": []
    },
    "displayName": "Display name",
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "orgRestrictions": [],
    "passwordCredentials": [],
    "preAuthorizedApplications": [],
    "requiredResourceAccess": [],
    "tags": [],
    "web": {
        "redirectUrls": [],
        "logoutUrl": null,
        "oauth2AllowImplicitFlow": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
