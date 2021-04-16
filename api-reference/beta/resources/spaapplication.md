---
title: тип ресурса spaApplication
description: Указывает параметры для одно-страницного приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 82848c5ea8427111b2d8b02c1886f3990faba79e
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836953"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="f221e-103">тип ресурса spaApplication</span><span class="sxs-lookup"><span data-stu-id="f221e-103">spaApplication resource type</span></span>

<span data-ttu-id="f221e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f221e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f221e-105">Указывает параметры для одно-страницного приложения.</span><span class="sxs-lookup"><span data-stu-id="f221e-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="f221e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f221e-106">Properties</span></span>

| <span data-ttu-id="f221e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f221e-107">Property</span></span> | <span data-ttu-id="f221e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f221e-108">Type</span></span> | <span data-ttu-id="f221e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f221e-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f221e-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="f221e-110">redirectUris</span></span> | <span data-ttu-id="f221e-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f221e-111">String collection</span></span> | <span data-ttu-id="f221e-112">Указывает URL-адреса, куда отправляются маркеры пользователей для регистрации, или URL-адреса перенаправления, куда отправляются коды авторизации OAuth 2.0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="f221e-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f221e-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f221e-113">JSON representation</span></span>
<span data-ttu-id="f221e-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f221e-114">The following is a JSON representation of the resource.</span></span>

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
