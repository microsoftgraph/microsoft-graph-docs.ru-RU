---
title: Тип ресурса Сервицеинформатион
description: Тип ресурса Сервицеинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ba13967a2b4373c1a3599baf2fcc856967fbb00c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939833"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="dc6e2-103">Тип ресурса Сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="dc6e2-103">serviceInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc6e2-104">Представляет базовые описательные данные о облачных службах, на которые пользователь выбрал ссылку из своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="dc6e2-104">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="dc6e2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc6e2-105">Properties</span></span>

| <span data-ttu-id="dc6e2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc6e2-106">Property</span></span>     | <span data-ttu-id="dc6e2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dc6e2-107">Type</span></span>        | <span data-ttu-id="dc6e2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dc6e2-108">Description</span></span>                                            |
|:-------------|:------------|:-------------------------------------------------------|
|<span data-ttu-id="dc6e2-109">name</span><span class="sxs-lookup"><span data-stu-id="dc6e2-109">name</span></span>          | <span data-ttu-id="dc6e2-110">String</span><span class="sxs-lookup"><span data-stu-id="dc6e2-110">String</span></span>      | <span data-ttu-id="dc6e2-111">Имя облачной службы (например, Twitter, Инстаграм).</span><span class="sxs-lookup"><span data-stu-id="dc6e2-111">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="dc6e2-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="dc6e2-112">webUrl</span></span>        | <span data-ttu-id="dc6e2-113">String</span><span class="sxs-lookup"><span data-stu-id="dc6e2-113">String</span></span>      | <span data-ttu-id="dc6e2-114">Содержит URL-адрес для службы, на которую указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="dc6e2-114">Contains the URL for the service being referenced.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="dc6e2-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc6e2-115">JSON representation</span></span>

<span data-ttu-id="dc6e2-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc6e2-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.serviceInformation",
  "baseType": null
}-->

```json
{
  "name": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
