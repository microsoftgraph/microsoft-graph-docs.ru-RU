---
title: Тип ресурса publicClientApplication
description: Задает параметры для веб-API без веб-приложения или веб-API. (например, мобильный или другой общедоступный клиент, например, установленное приложение, запущенное на настольном устройстве)
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e22f973f9d133b3c4c7827733f51f2028cd506ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521308"
---
# <a name="publicclientapplication-resource-type"></a><span data-ttu-id="b043f-104">Тип ресурса publicClientApplication</span><span class="sxs-lookup"><span data-stu-id="b043f-104">publicClientApplication resource type</span></span>

<span data-ttu-id="b043f-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b043f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b043f-106">Задает параметры для невеб-приложения или API, не являющихся веб-приложениями (например, мобильных или других общедоступных клиентов, таких как установленное приложение, запущенное на настольном устройстве).</span><span class="sxs-lookup"><span data-stu-id="b043f-106">Specifies settings for non-web app or non-web API (for example, mobile or other public clients such as an installed application running on a desktop device).</span></span>

## <a name="properties"></a><span data-ttu-id="b043f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b043f-107">Properties</span></span>

| <span data-ttu-id="b043f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b043f-108">Property</span></span> | <span data-ttu-id="b043f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b043f-109">Type</span></span> | <span data-ttu-id="b043f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b043f-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b043f-111">редиректурис</span><span class="sxs-lookup"><span data-stu-id="b043f-111">redirectUris</span></span>|<span data-ttu-id="b043f-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b043f-112">String collection</span></span>| <span data-ttu-id="b043f-113">Задает URL-адреса, по которым маркеры пользователей отправляются для входа, или URI перенаправления, для которых отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="b043f-113">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b043f-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b043f-114">JSON representation</span></span>
<span data-ttu-id="b043f-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b043f-115">Here is a JSON representation of the resource.</span></span>

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
