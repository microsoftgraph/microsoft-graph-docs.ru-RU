---
title: Тип ресурса publicClientApplication
description: Задает параметры для веб-API без веб-приложения или веб-API. (например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e25c61cc58874944017ee34dddcff75c22b134b6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937415"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="801d6-104">Тип ресурса publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="801d6-104">publicClientApplication resource type</span></span>

<span data-ttu-id="801d6-105">Задает параметры для невеб-приложения или API, не являющихся веб-приложениями (например, мобильных или других общедоступных клиентов, таких как установленное приложение, запущенное на настольном устройстве).</span><span class="sxs-lookup"><span data-stu-id="801d6-105">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="801d6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="801d6-106">Properties</span></span>

| <span data-ttu-id="801d6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="801d6-107">Property</span></span> | <span data-ttu-id="801d6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="801d6-108">Type</span></span> | <span data-ttu-id="801d6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="801d6-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="801d6-110">редиректурис</span><span class="sxs-lookup"><span data-stu-id="801d6-110">redirectUris</span></span>|<span data-ttu-id="801d6-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="801d6-111">String collection</span></span>| <span data-ttu-id="801d6-112">Задает URL-адреса, по которым маркеры пользователей отправляются для входа, или URI перенаправления, для которых отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="801d6-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="801d6-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="801d6-113">JSON representation</span></span>
<span data-ttu-id="801d6-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="801d6-114">Here is a JSON representation of the resource.</span></span>

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
