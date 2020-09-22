---
title: Тип ресурса Сервицеинформатион
description: Тип ресурса Сервицеинформатион
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 39382b0fb17795bde26b4e54f629b2e4281f81db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070445"
---
# <a name="serviceinformation-resource-type"></a><span data-ttu-id="90f4e-103">Тип ресурса Сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="90f4e-103">serviceInformation resource type</span></span>

<span data-ttu-id="90f4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90f4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90f4e-105">Представляет базовые описательные данные о облачных службах, на которые пользователь выбрал ссылку из своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="90f4e-105">Represents basic descriptive data about cloud services that a user has chosen to refer to from their account.</span></span>

## <a name="properties"></a><span data-ttu-id="90f4e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="90f4e-106">Properties</span></span>

| <span data-ttu-id="90f4e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="90f4e-107">Property</span></span>     | <span data-ttu-id="90f4e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="90f4e-108">Type</span></span>        | <span data-ttu-id="90f4e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="90f4e-109">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="90f4e-110">name</span><span class="sxs-lookup"><span data-stu-id="90f4e-110">name</span></span>          | <span data-ttu-id="90f4e-111">String</span><span class="sxs-lookup"><span data-stu-id="90f4e-111">String</span></span>      | <span data-ttu-id="90f4e-112">Имя облачной службы (например, Twitter, Инстаграм).</span><span class="sxs-lookup"><span data-stu-id="90f4e-112">The name of the cloud service (for example, Twitter, Instagram).</span></span> |
|<span data-ttu-id="90f4e-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="90f4e-113">webUrl</span></span>        | <span data-ttu-id="90f4e-114">String</span><span class="sxs-lookup"><span data-stu-id="90f4e-114">String</span></span>      | <span data-ttu-id="90f4e-115">Содержит URL-адрес для службы, на которую указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="90f4e-115">Contains the URL for the service being referenced.</span></span>               |

## <a name="json-representation"></a><span data-ttu-id="90f4e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90f4e-116">JSON representation</span></span>

<span data-ttu-id="90f4e-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90f4e-117">The following is a JSON representation of the resource.</span></span>

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


