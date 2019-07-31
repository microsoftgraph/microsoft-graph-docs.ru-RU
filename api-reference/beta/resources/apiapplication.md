---
title: Тип ресурса API
description: Задает параметры для приложения веб-API.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3bf5ffc21c13e0952efd0f5ea773f76dc3f7b46f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974341"
---
# <a name="api-resource-type"></a><span data-ttu-id="a395d-103">Тип ресурса API</span><span class="sxs-lookup"><span data-stu-id="a395d-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a395d-104">Задает параметры для приложения веб-API.</span><span class="sxs-lookup"><span data-stu-id="a395d-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="a395d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a395d-105">Properties</span></span>

| <span data-ttu-id="a395d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a395d-106">Property</span></span> | <span data-ttu-id="a395d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a395d-107">Type</span></span> | <span data-ttu-id="a395d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a395d-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a395d-109">Рекуестедакцесстокенверсион</span><span class="sxs-lookup"><span data-stu-id="a395d-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="a395d-110">Int32</span><span class="sxs-lookup"><span data-stu-id="a395d-110">Int32</span></span>| <span data-ttu-id="a395d-111">Указывает принятую версию маркера доступа для текущего ресурса API.</span><span class="sxs-lookup"><span data-stu-id="a395d-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="a395d-112">Возможные значения: 1 или 2.</span><span class="sxs-lookup"><span data-stu-id="a395d-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="a395d-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="a395d-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="a395d-114">Коллекция [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="a395d-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="a395d-115">Коллекция областей разрешений OAuth 2,0, предоставляемых приложением веб-API (ресурсом) для клиентских приложений.</span><span class="sxs-lookup"><span data-stu-id="a395d-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="a395d-116">Эти области разрешений могут быть назначены клиентским приложениям во время согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="a395d-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a395d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a395d-117">JSON representation</span></span>
<span data-ttu-id="a395d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a395d-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
