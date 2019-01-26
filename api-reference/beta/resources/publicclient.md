---
title: Тип ресурса publicClient
description: Задает параметры для без веб-приложения или веб-Api. (например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)
localization_priority: Normal
ms.openlocfilehash: 866e27b4ea3e1386b7cc69f967635d38641f121c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571844"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="160ab-104">Тип ресурса publicClient</span><span class="sxs-lookup"><span data-stu-id="160ab-104">publicClient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="160ab-105">Задает параметры для без веб-приложения или веб-Api.</span><span class="sxs-lookup"><span data-stu-id="160ab-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="160ab-106">(например, Mobile или других общедоступных клиентом, например установленные приложения, запущенного на устройстве настольных систем)</span><span class="sxs-lookup"><span data-stu-id="160ab-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="160ab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="160ab-107">Properties</span></span>

| <span data-ttu-id="160ab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="160ab-108">Property</span></span> | <span data-ttu-id="160ab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="160ab-109">Type</span></span> | <span data-ttu-id="160ab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="160ab-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="160ab-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="160ab-111">redirectUris</span></span>|<span data-ttu-id="160ab-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="160ab-112">String collection</span></span>| <span data-ttu-id="160ab-113">Указывает URL-адресов, которые будут отправлены маркеры пользователя для входа в или отправки коды авторизации коды URI, OAuth 2.0 и маркеры доступа для перенаправления.</span><span class="sxs-lookup"><span data-stu-id="160ab-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="160ab-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="160ab-114">JSON representation</span></span>
<span data-ttu-id="160ab-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="160ab-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicClientApplication"
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
