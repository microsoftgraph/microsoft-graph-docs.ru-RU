---
title: Тип ресурса API
description: Задает параметры для приложения веб-API.
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535693"
---
# <a name="api-resource-type"></a><span data-ttu-id="916f3-103">Тип ресурса API</span><span class="sxs-lookup"><span data-stu-id="916f3-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="916f3-104">Задает параметры для приложения веб-API.</span><span class="sxs-lookup"><span data-stu-id="916f3-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="916f3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="916f3-105">Properties</span></span>

| <span data-ttu-id="916f3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="916f3-106">Property</span></span> | <span data-ttu-id="916f3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="916f3-107">Type</span></span> | <span data-ttu-id="916f3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="916f3-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="916f3-109">Рекуестедакцесстокенверсион</span><span class="sxs-lookup"><span data-stu-id="916f3-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="916f3-110">Int32</span><span class="sxs-lookup"><span data-stu-id="916f3-110">Int32</span></span>| <span data-ttu-id="916f3-111">Указывает принятую версию маркера доступа для текущего ресурса API.</span><span class="sxs-lookup"><span data-stu-id="916f3-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="916f3-112">Возможные значения: 1 или 2.</span><span class="sxs-lookup"><span data-stu-id="916f3-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="916f3-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="916f3-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="916f3-114">Коллекция [permissionScope](permissionscope.md)</span><span class="sxs-lookup"><span data-stu-id="916f3-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="916f3-115">Коллекция областей разрешений OAuth 2,0, предоставляемых приложением веб-API (ресурсом) для клиентских приложений.</span><span class="sxs-lookup"><span data-stu-id="916f3-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="916f3-116">Эти области разрешений могут быть назначены клиентским приложениям во время согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="916f3-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="916f3-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="916f3-117">JSON representation</span></span>
<span data-ttu-id="916f3-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="916f3-118">Here is a JSON representation of the resource.</span></span>

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
