---
title: Тип ресурса spaApplication
description: Указывает параметры для одно страниц приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: hamiltonha
ms.openlocfilehash: a05d2eb997212b3baf88b84e21468475a45a691c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128829"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="e2310-103">Тип ресурса spaApplication</span><span class="sxs-lookup"><span data-stu-id="e2310-103">spaApplication resource type</span></span>

<span data-ttu-id="e2310-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2310-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2310-105">Указывает параметры для одно страниц приложения.</span><span class="sxs-lookup"><span data-stu-id="e2310-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="e2310-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2310-106">Properties</span></span>

| <span data-ttu-id="e2310-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2310-107">Property</span></span> | <span data-ttu-id="e2310-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e2310-108">Type</span></span> | <span data-ttu-id="e2310-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e2310-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e2310-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="e2310-110">redirectUris</span></span> | <span data-ttu-id="e2310-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e2310-111">String collection</span></span> | <span data-ttu-id="e2310-112">Указывает URL-адреса, в которые отправляются маркеры пользователей для входов, или URIS перенаправления, в которые отправляются коды авторизации OAuth 2.0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="e2310-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2310-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e2310-113">JSON representation</span></span>
<span data-ttu-id="e2310-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2310-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.spaApplication"
}-->

```json
{
  "redirectUris": ["String"]
}
```
