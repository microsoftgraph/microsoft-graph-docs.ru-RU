---
title: Тип ресурса Информатионпротектионконтентлабел
description: Описывает объект Информатионпротектионконтентлабел, определяющий метаданные МИП для объекта.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4f615655110ffdc6b76469d3d29cd4d13663d511
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938830"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="42ebd-103">Тип ресурса Информатионпротектионконтентлабел</span><span class="sxs-lookup"><span data-stu-id="42ebd-103">informationProtectionContentLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42ebd-104">Описывает объект Информатионпротектионконтентлабел, определяющий метаданные МИП для объекта.</span><span class="sxs-lookup"><span data-stu-id="42ebd-104">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="42ebd-105">**информатионпротектионконтентлабел** возвращается с помощью API [екстрактлабел](../api/informationprotectionlabel-extractLabel.md) , который разрешается в метку, которая в данный момент применена к файлу.</span><span class="sxs-lookup"><span data-stu-id="42ebd-105">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="42ebd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="42ebd-106">Properties</span></span>

| <span data-ttu-id="42ebd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="42ebd-107">Property</span></span>     | <span data-ttu-id="42ebd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="42ebd-108">Type</span></span>        | <span data-ttu-id="42ebd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="42ebd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42ebd-110">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="42ebd-110">assignmentMethod</span></span>|<span data-ttu-id="42ebd-111">Строка</span><span class="sxs-lookup"><span data-stu-id="42ebd-111">String</span></span>| <span data-ttu-id="42ebd-112">Возможные значения: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="42ebd-112">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="42ebd-113">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="42ebd-113">creationDateTime</span></span>|<span data-ttu-id="42ebd-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42ebd-114">DateTimeOffset</span></span>|<span data-ttu-id="42ebd-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="42ebd-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="42ebd-117">label</span><span class="sxs-lookup"><span data-stu-id="42ebd-117">label</span></span>|[<span data-ttu-id="42ebd-118">лабелдетаилс</span><span class="sxs-lookup"><span data-stu-id="42ebd-118">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="42ebd-119">Сведения о метке, которая в настоящее время применяется к файлу.</span><span class="sxs-lookup"><span data-stu-id="42ebd-119">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42ebd-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42ebd-120">JSON representation</span></span>

<span data-ttu-id="42ebd-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42ebd-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.informationProtectionContentLabel",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "creationDateTime": "String (timestamp)",
  "label": {"@odata.type": "microsoft.graph.labelDetails"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionContentLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->