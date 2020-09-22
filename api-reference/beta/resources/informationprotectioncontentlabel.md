---
title: Тип ресурса Информатионпротектионконтентлабел
description: Описывает объект Информатионпротектионконтентлабел, определяющий метаданные МИП для объекта.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8422f83db0c94eed74d5690343c51b70e2d87d82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016452"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="d4d8c-103">Тип ресурса Информатионпротектионконтентлабел</span><span class="sxs-lookup"><span data-stu-id="d4d8c-103">informationProtectionContentLabel resource type</span></span>

<span data-ttu-id="d4d8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4d8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4d8c-105">Описывает объект Информатионпротектионконтентлабел, определяющий метаданные МИП для объекта.</span><span class="sxs-lookup"><span data-stu-id="d4d8c-105">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="d4d8c-106">**информатионпротектионконтентлабел** возвращается с помощью API [екстрактлабел](../api/informationprotectionlabel-extractLabel.md) , который разрешается в метку, которая в данный момент применена к файлу.</span><span class="sxs-lookup"><span data-stu-id="d4d8c-106">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="d4d8c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4d8c-107">Properties</span></span>

| <span data-ttu-id="d4d8c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4d8c-108">Property</span></span>     | <span data-ttu-id="d4d8c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d4d8c-109">Type</span></span>        | <span data-ttu-id="d4d8c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d4d8c-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4d8c-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="d4d8c-111">assignmentMethod</span></span>|<span data-ttu-id="d4d8c-112">String</span><span class="sxs-lookup"><span data-stu-id="d4d8c-112">String</span></span>| <span data-ttu-id="d4d8c-113">Возможные значения: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="d4d8c-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="d4d8c-114">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="d4d8c-114">creationDateTime</span></span>|<span data-ttu-id="d4d8c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4d8c-115">DateTimeOffset</span></span>|<span data-ttu-id="d4d8c-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d4d8c-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d4d8c-118">label</span><span class="sxs-lookup"><span data-stu-id="d4d8c-118">label</span></span>|[<span data-ttu-id="d4d8c-119">лабелдетаилс</span><span class="sxs-lookup"><span data-stu-id="d4d8c-119">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="d4d8c-120">Сведения о метке, которая в настоящее время применяется к файлу.</span><span class="sxs-lookup"><span data-stu-id="d4d8c-120">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4d8c-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4d8c-121">JSON representation</span></span>

<span data-ttu-id="d4d8c-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4d8c-122">The following is a JSON representation of the resource.</span></span>

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

