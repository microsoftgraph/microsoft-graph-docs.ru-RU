---
title: Тип ресурса publicClient
description: Задает параметры для без веб-приложения или веб-Api. (например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)
localization_priority: Normal
ms.openlocfilehash: ff1d77709293a7167868451671e1660196c9a4db
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525964"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="cf827-104">Тип ресурса publicClient</span><span class="sxs-lookup"><span data-stu-id="cf827-104">publicClient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf827-105">Задает параметры для без веб-приложения или веб-Api.</span><span class="sxs-lookup"><span data-stu-id="cf827-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="cf827-106">(например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)</span><span class="sxs-lookup"><span data-stu-id="cf827-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="cf827-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf827-107">Properties</span></span>

| <span data-ttu-id="cf827-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf827-108">Property</span></span> | <span data-ttu-id="cf827-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cf827-109">Type</span></span> | <span data-ttu-id="cf827-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cf827-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cf827-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="cf827-111">redirectUris</span></span>|<span data-ttu-id="cf827-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cf827-112">String collection</span></span>| <span data-ttu-id="cf827-113">Указывает URL-адресов, которые будут отправлены маркеры пользователя для входа в или отправки коды авторизации коды URI, OAuth 2.0 и маркеры доступа для перенаправления.</span><span class="sxs-lookup"><span data-stu-id="cf827-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf827-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf827-114">JSON representation</span></span>
<span data-ttu-id="cf827-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf827-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
