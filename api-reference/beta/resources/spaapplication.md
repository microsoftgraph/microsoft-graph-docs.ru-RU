---
title: Тип ресурса Спааппликатион
description: Задает параметры для одностраничного приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: hamiltonha
ms.openlocfilehash: dd5e2c6419acd66cb482f2ccff2914b1bf0245dc
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031950"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="18a21-103">Тип ресурса Спааппликатион</span><span class="sxs-lookup"><span data-stu-id="18a21-103">spaApplication resource type</span></span>

<span data-ttu-id="18a21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18a21-105">Задает параметры для одностраничного приложения.</span><span class="sxs-lookup"><span data-stu-id="18a21-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="18a21-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="18a21-106">Properties</span></span>

| <span data-ttu-id="18a21-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="18a21-107">Property</span></span> | <span data-ttu-id="18a21-108">Тип</span><span class="sxs-lookup"><span data-stu-id="18a21-108">Type</span></span> | <span data-ttu-id="18a21-109">Описание</span><span class="sxs-lookup"><span data-stu-id="18a21-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="18a21-110">редиректурис</span><span class="sxs-lookup"><span data-stu-id="18a21-110">redirectUris</span></span> | <span data-ttu-id="18a21-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="18a21-111">String collection</span></span> | <span data-ttu-id="18a21-112">Задает URL-адреса, по которым маркеры пользователей отправляются для входа, или URI перенаправления, для которых отправляются коды авторизации OAuth 2,0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="18a21-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18a21-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18a21-113">JSON representation</span></span>
<span data-ttu-id="18a21-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18a21-114">The following is a JSON representation of the resource.</span></span>

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
