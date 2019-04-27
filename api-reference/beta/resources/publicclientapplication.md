---
title: Тип ресурса publicClientApplication
description: Задает параметры для веб-API без веб-приложения или веб-API. (например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
ms.openlocfilehash: 8118d1e771cb55ce5b82c9ddac14aaa45260ab56
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348965"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="92e8e-104">Тип ресурса publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="92e8e-104">publicClientApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92e8e-105">Задает параметры для веб-API без веб-приложения или веб-API.</span><span class="sxs-lookup"><span data-stu-id="92e8e-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="92e8e-106">(например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)</span><span class="sxs-lookup"><span data-stu-id="92e8e-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="92e8e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="92e8e-107">Properties</span></span>

| <span data-ttu-id="92e8e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="92e8e-108">Property</span></span> | <span data-ttu-id="92e8e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="92e8e-109">Type</span></span> | <span data-ttu-id="92e8e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92e8e-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="92e8e-111">Редиректурис</span><span class="sxs-lookup"><span data-stu-id="92e8e-111">redirectUris</span></span>|<span data-ttu-id="92e8e-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="92e8e-112">String collection</span></span>| <span data-ttu-id="92e8e-113">Задает URL-адреса, на которые отправляются маркеры пользователей для входа, или URI перенаправления, на которые отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="92e8e-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92e8e-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92e8e-114">JSON representation</span></span>
<span data-ttu-id="92e8e-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92e8e-115">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
