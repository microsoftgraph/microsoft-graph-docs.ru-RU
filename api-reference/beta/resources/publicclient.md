---
title: Тип ресурса publicClient
description: Задает параметры для веб-API без веб-приложения или веб-API. (например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
ms.openlocfilehash: ff1d77709293a7167868451671e1660196c9a4db
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563370"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="09309-104">Тип ресурса publicClient</span><span class="sxs-lookup"><span data-stu-id="09309-104">publicClient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09309-105">Задает параметры для веб-API без веб-приложения или веб-API.</span><span class="sxs-lookup"><span data-stu-id="09309-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="09309-106">(например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)</span><span class="sxs-lookup"><span data-stu-id="09309-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="09309-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="09309-107">Properties</span></span>

| <span data-ttu-id="09309-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="09309-108">Property</span></span> | <span data-ttu-id="09309-109">Тип</span><span class="sxs-lookup"><span data-stu-id="09309-109">Type</span></span> | <span data-ttu-id="09309-110">Описание</span><span class="sxs-lookup"><span data-stu-id="09309-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="09309-111">Редиректурис</span><span class="sxs-lookup"><span data-stu-id="09309-111">redirectUris</span></span>|<span data-ttu-id="09309-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="09309-112">String collection</span></span>| <span data-ttu-id="09309-113">Задает URL-адреса, на которые отправляются маркеры пользователей для входа, или URI перенаправления, на которые отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="09309-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09309-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09309-114">JSON representation</span></span>
<span data-ttu-id="09309-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09309-115">Here is a JSON representation of the resource.</span></span>

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
