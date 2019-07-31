---
title: Тип ресурса publicClientApplication
description: Задает параметры для веб-API без веб-приложения или веб-API. (например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4503e65777b41fc2f864cd818697b048e3c8e435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965560"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="e0a9b-104">Тип ресурса publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="e0a9b-104">publicClientApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0a9b-105">Задает параметры для веб-API без веб-приложения или веб-API.</span><span class="sxs-lookup"><span data-stu-id="e0a9b-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="e0a9b-106">(например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)</span><span class="sxs-lookup"><span data-stu-id="e0a9b-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="e0a9b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0a9b-107">Properties</span></span>

| <span data-ttu-id="e0a9b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0a9b-108">Property</span></span> | <span data-ttu-id="e0a9b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e0a9b-109">Type</span></span> | <span data-ttu-id="e0a9b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e0a9b-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a9b-111">Редиректурис</span><span class="sxs-lookup"><span data-stu-id="e0a9b-111">redirectUris</span></span>|<span data-ttu-id="e0a9b-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e0a9b-112">String collection</span></span>| <span data-ttu-id="e0a9b-113">Задает URL-адреса, на которые отправляются маркеры пользователей для входа, или URI перенаправления, на которые отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="e0a9b-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e0a9b-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0a9b-114">JSON representation</span></span>
<span data-ttu-id="e0a9b-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0a9b-115">Here is a JSON representation of the resource.</span></span>

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
