---
title: Тип ресурса Персондатасаурце
description: Представляет источники, из которых берутся данные пользователя, например каталог и контакты Outlook.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: b4cf88dc64010e900bf3b37061f27b3ffb6f3908
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344961"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="e1861-103">Тип ресурса Персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="e1861-103">personDataSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1861-104">Представляет источники, из которых берутся данные пользователя, например каталог и контакты Outlook.</span><span class="sxs-lookup"><span data-stu-id="e1861-104">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1861-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1861-105">JSON representation</span></span>

<span data-ttu-id="e1861-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e1861-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e1861-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1861-107">Properties</span></span>
| <span data-ttu-id="e1861-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1861-108">Property</span></span>     | <span data-ttu-id="e1861-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e1861-109">Type</span></span>   |<span data-ttu-id="e1861-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e1861-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1861-111">type</span><span class="sxs-lookup"><span data-stu-id="e1861-111">type</span></span>|<span data-ttu-id="e1861-112">String</span><span class="sxs-lookup"><span data-stu-id="e1861-112">String</span></span>|<span data-ttu-id="e1861-113">Тип источника данных.</span><span class="sxs-lookup"><span data-stu-id="e1861-113">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
