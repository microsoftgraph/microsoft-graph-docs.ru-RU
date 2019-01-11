---
title: Тип ресурса API
description: Задает параметры для приложения Web API.
localization_priority: Normal
ms.openlocfilehash: 50c21c31fec7434514408e1a214c6edf2b838c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845210"
---
# <a name="api-resource-type"></a><span data-ttu-id="3c42d-103">Тип ресурса API</span><span class="sxs-lookup"><span data-stu-id="3c42d-103">api resource type</span></span>

> <span data-ttu-id="3c42d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c42d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c42d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c42d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c42d-106">Задает параметры для приложения Web API.</span><span class="sxs-lookup"><span data-stu-id="3c42d-106">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="3c42d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c42d-107">Properties</span></span>

| <span data-ttu-id="3c42d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c42d-108">Property</span></span> | <span data-ttu-id="3c42d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3c42d-109">Type</span></span> | <span data-ttu-id="3c42d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c42d-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3c42d-111">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="3c42d-111">requestedAccessTokenVersion</span></span>|<span data-ttu-id="3c42d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="3c42d-112">Int32</span></span>| <span data-ttu-id="3c42d-113">Указывает версию маркера обслуживаемых доступа для текущего ресурса API.</span><span class="sxs-lookup"><span data-stu-id="3c42d-113">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="3c42d-114">Возможные значения: 1 или 2.</span><span class="sxs-lookup"><span data-stu-id="3c42d-114">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="3c42d-115">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="3c42d-115">oauth2PermissionScopes</span></span>|<span data-ttu-id="3c42d-116">[permissionScope](permissionscope.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3c42d-116">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="3c42d-117">Коллекция OAuth 2.0 области разрешений, предоставляемых веб-приложению API (ресурс) на клиентские приложения.</span><span class="sxs-lookup"><span data-stu-id="3c42d-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="3c42d-118">Эти области разрешений могут быть предоставлены на клиентские приложения во время подтверждения.</span><span class="sxs-lookup"><span data-stu-id="3c42d-118">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3c42d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c42d-119">JSON representation</span></span>
<span data-ttu-id="3c42d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c42d-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
