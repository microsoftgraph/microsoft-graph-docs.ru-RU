---
title: Тип ресурса publicClientApplication
description: Указывает параметры для других веб-приложений и веб-API. (Например, мобильный или другой общедоступный клиент, например установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: a15f0ea159ab12403186465783200a9e374562bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137517"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="6e7d6-104">Тип ресурса publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="6e7d6-104">publicClientApplication resource type</span></span>

<span data-ttu-id="6e7d6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e7d6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e7d6-106">Указывает параметры для не веб-приложения или не-веб-API (например, мобильных или других общедоступных клиентов, таких как установленное приложение, запущенное на настольном устройстве).</span><span class="sxs-lookup"><span data-stu-id="6e7d6-106">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="6e7d6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e7d6-107">Properties</span></span>

| <span data-ttu-id="6e7d6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e7d6-108">Property</span></span> | <span data-ttu-id="6e7d6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e7d6-109">Type</span></span> | <span data-ttu-id="6e7d6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e7d6-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6e7d6-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="6e7d6-111">redirectUris</span></span>|<span data-ttu-id="6e7d6-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6e7d6-112">String collection</span></span>| <span data-ttu-id="6e7d6-113">Указывает URL-адреса, в которые отправляются маркеры пользователей для входов, или IS перенаправления, в которые отправляются коды авторизации OAuth 2.0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="6e7d6-113">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e7d6-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e7d6-114">JSON representation</span></span>
<span data-ttu-id="6e7d6-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e7d6-115">Here is a JSON representation of the resource.</span></span>

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

