---
title: тип ресурса spaApplication
description: Указывает параметры для одно-страницного приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 25f907aa8c7e5b47960bb3a482b9745c488d16a9
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836988"
---
# <a name="spaapplication-resource-type"></a><span data-ttu-id="efb45-103">тип ресурса spaApplication</span><span class="sxs-lookup"><span data-stu-id="efb45-103">spaApplication resource type</span></span>

<span data-ttu-id="efb45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efb45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efb45-105">Указывает параметры для одно-страницного приложения.</span><span class="sxs-lookup"><span data-stu-id="efb45-105">Specifies settings for a single-page application.</span></span>

## <a name="properties"></a><span data-ttu-id="efb45-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="efb45-106">Properties</span></span>

| <span data-ttu-id="efb45-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="efb45-107">Property</span></span> | <span data-ttu-id="efb45-108">Тип</span><span class="sxs-lookup"><span data-stu-id="efb45-108">Type</span></span> | <span data-ttu-id="efb45-109">Описание</span><span class="sxs-lookup"><span data-stu-id="efb45-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="efb45-110">redirectUris</span><span class="sxs-lookup"><span data-stu-id="efb45-110">redirectUris</span></span> | <span data-ttu-id="efb45-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="efb45-111">String collection</span></span> | <span data-ttu-id="efb45-112">Указывает URL-адреса, куда отправляются маркеры пользователей для регистрации, или URL-адреса перенаправления, куда отправляются коды авторизации OAuth 2.0 и маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="efb45-112">Specifies the URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="efb45-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efb45-113">JSON representation</span></span>
<span data-ttu-id="efb45-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efb45-114">The following is a JSON representation of the resource.</span></span>

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
