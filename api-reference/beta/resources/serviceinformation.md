---
title: Тип ресурса Сервицеинформатион
description: Тип ресурса Сервицеинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7b121a1bd3369eebd752651fa412510daf943b76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520789"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="8896b-103">Тип ресурса Сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="8896b-103">serviceInformation resource type</span></span>

<span data-ttu-id="8896b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8896b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8896b-105">Представляет базовые описательные данные о облачных службах, на которые пользователь выбрал ссылку из своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="8896b-105">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="8896b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8896b-106">Properties</span></span>

| <span data-ttu-id="8896b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8896b-107">Property</span></span>     | <span data-ttu-id="8896b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8896b-108">Type</span></span>        | <span data-ttu-id="8896b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8896b-109">Description</span></span>                                            |
|:-------------|:------------|:-------------------------------------------------------|
|<span data-ttu-id="8896b-110">name</span><span class="sxs-lookup"><span data-stu-id="8896b-110">name</span></span>          | <span data-ttu-id="8896b-111">String</span><span class="sxs-lookup"><span data-stu-id="8896b-111">String</span></span>      | <span data-ttu-id="8896b-112">Имя облачной службы (например, Twitter, Инстаграм).</span><span class="sxs-lookup"><span data-stu-id="8896b-112">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="8896b-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="8896b-113">webUrl</span></span>        | <span data-ttu-id="8896b-114">String</span><span class="sxs-lookup"><span data-stu-id="8896b-114">String</span></span>      | <span data-ttu-id="8896b-115">Содержит URL-адрес для службы, на которую указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="8896b-115">Contains the URL for the service being referenced.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="8896b-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8896b-116">JSON representation</span></span>

<span data-ttu-id="8896b-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8896b-117">The following is a JSON representation of the resource.</span></span>

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
