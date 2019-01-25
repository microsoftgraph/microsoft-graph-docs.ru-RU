---
title: Тип ресурса API
description: Задает параметры для приложения Web API.
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521448"
---
# <a name="api-resource-type"></a><span data-ttu-id="3ebab-103">Тип ресурса API</span><span class="sxs-lookup"><span data-stu-id="3ebab-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ebab-104">Задает параметры для приложения Web API.</span><span class="sxs-lookup"><span data-stu-id="3ebab-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="3ebab-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ebab-105">Properties</span></span>

| <span data-ttu-id="3ebab-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ebab-106">Property</span></span> | <span data-ttu-id="3ebab-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3ebab-107">Type</span></span> | <span data-ttu-id="3ebab-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3ebab-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3ebab-109">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="3ebab-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="3ebab-110">Int32</span><span class="sxs-lookup"><span data-stu-id="3ebab-110">Int32</span></span>| <span data-ttu-id="3ebab-111">Указывает версию маркера обслуживаемых доступа для текущего ресурса API.</span><span class="sxs-lookup"><span data-stu-id="3ebab-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="3ebab-112">Возможные значения: 1 или 2.</span><span class="sxs-lookup"><span data-stu-id="3ebab-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="3ebab-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="3ebab-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="3ebab-114">[permissionScope](permissionscope.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3ebab-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="3ebab-115">Коллекция OAuth 2.0 области разрешений, предоставляемых веб-приложению API (ресурс) на клиентские приложения.</span><span class="sxs-lookup"><span data-stu-id="3ebab-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="3ebab-116">Эти области разрешений могут быть предоставлены на клиентские приложения во время подтверждения.</span><span class="sxs-lookup"><span data-stu-id="3ebab-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3ebab-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ebab-117">JSON representation</span></span>
<span data-ttu-id="3ebab-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ebab-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/api.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
