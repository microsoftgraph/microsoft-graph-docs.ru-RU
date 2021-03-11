---
title: тип ресурса informationProtectionContentLabel
description: Описывает объект informationProtectionContentLabel, который определяет метаданные MIP на объекте.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a7905a585b28832829d838db94344b28f691644d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718543"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="86a62-103">тип ресурса informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="86a62-103">informationProtectionContentLabel resource type</span></span>

<span data-ttu-id="86a62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86a62-105">Описывает объект informationProtectionContentLabel, который определяет метаданные MIP на объекте.</span><span class="sxs-lookup"><span data-stu-id="86a62-105">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="86a62-106">**informationProtectionContentLabel** возвращается [решением API extractLabel](../api/informationprotectionlabel-extractLabel.md) на метку, которая в настоящее время применяется к файлу.</span><span class="sxs-lookup"><span data-stu-id="86a62-106">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="86a62-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86a62-107">Properties</span></span>

| <span data-ttu-id="86a62-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86a62-108">Property</span></span>     | <span data-ttu-id="86a62-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86a62-109">Type</span></span>        | <span data-ttu-id="86a62-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86a62-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86a62-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="86a62-111">assignmentMethod</span></span>|<span data-ttu-id="86a62-112">String</span><span class="sxs-lookup"><span data-stu-id="86a62-112">String</span></span>| <span data-ttu-id="86a62-113">Возможные значения: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="86a62-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="86a62-114">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="86a62-114">creationDateTime</span></span>|<span data-ttu-id="86a62-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86a62-115">DateTimeOffset</span></span>|<span data-ttu-id="86a62-116">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="86a62-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="86a62-117">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="86a62-117">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="86a62-118">label</span><span class="sxs-lookup"><span data-stu-id="86a62-118">label</span></span>|[<span data-ttu-id="86a62-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="86a62-119">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="86a62-120">Сведения о мете, которая в настоящее время применяется к файлу.</span><span class="sxs-lookup"><span data-stu-id="86a62-120">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86a62-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86a62-121">JSON representation</span></span>

<span data-ttu-id="86a62-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86a62-122">The following is a JSON representation of the resource.</span></span>

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

