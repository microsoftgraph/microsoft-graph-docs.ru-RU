---
title: Тип ресурса Информатионпротектионконтентлабел
description: Описывает объект Информатионпротектионконтентлабел, определяющий метаданные МИП для объекта.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 454dd6dd3b095c01e476f52ae38d3a9caa552192
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496084"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="45afe-103">Тип ресурса Информатионпротектионконтентлабел</span><span class="sxs-lookup"><span data-stu-id="45afe-103">informationProtectionContentLabel resource type</span></span>

<span data-ttu-id="45afe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45afe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45afe-105">Описывает объект Информатионпротектионконтентлабел, определяющий метаданные МИП для объекта.</span><span class="sxs-lookup"><span data-stu-id="45afe-105">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="45afe-106">**информатионпротектионконтентлабел** возвращается с помощью API [екстрактлабел](../api/informationprotectionlabel-extractLabel.md) , который разрешается в метку, которая в данный момент применена к файлу.</span><span class="sxs-lookup"><span data-stu-id="45afe-106">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="45afe-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="45afe-107">Properties</span></span>

| <span data-ttu-id="45afe-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="45afe-108">Property</span></span>     | <span data-ttu-id="45afe-109">Тип</span><span class="sxs-lookup"><span data-stu-id="45afe-109">Type</span></span>        | <span data-ttu-id="45afe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="45afe-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="45afe-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="45afe-111">assignmentMethod</span></span>|<span data-ttu-id="45afe-112">Строка</span><span class="sxs-lookup"><span data-stu-id="45afe-112">String</span></span>| <span data-ttu-id="45afe-113">Возможные значения: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="45afe-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="45afe-114">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="45afe-114">creationDateTime</span></span>|<span data-ttu-id="45afe-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45afe-115">DateTimeOffset</span></span>|<span data-ttu-id="45afe-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="45afe-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="45afe-118">label</span><span class="sxs-lookup"><span data-stu-id="45afe-118">label</span></span>|[<span data-ttu-id="45afe-119">лабелдетаилс</span><span class="sxs-lookup"><span data-stu-id="45afe-119">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="45afe-120">Сведения о метке, которая в настоящее время применяется к файлу.</span><span class="sxs-lookup"><span data-stu-id="45afe-120">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45afe-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45afe-121">JSON representation</span></span>

<span data-ttu-id="45afe-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45afe-122">The following is a JSON representation of the resource.</span></span>

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