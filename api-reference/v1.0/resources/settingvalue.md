---
title: Тип ресурса settingValue
description: Параметр, представленный парой "имя-значение".
ms.openlocfilehash: b47c5c746117390cfd59db71d832928e482403b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028479"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="dbde8-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="dbde8-103">settingValue resource type</span></span>

<span data-ttu-id="dbde8-104">Параметр, представленный парой "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="dbde8-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="dbde8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbde8-105">Properties</span></span>

| <span data-ttu-id="dbde8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbde8-106">Property</span></span> | <span data-ttu-id="dbde8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dbde8-107">Type</span></span> | <span data-ttu-id="dbde8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dbde8-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dbde8-109">name</span><span class="sxs-lookup"><span data-stu-id="dbde8-109">name</span></span>|<span data-ttu-id="dbde8-110">String</span><span class="sxs-lookup"><span data-stu-id="dbde8-110">String</span></span>| <span data-ttu-id="dbde8-111">Имя параметра, определенное [groupSettingTemplate](groupsettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="dbde8-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="dbde8-112">value</span><span class="sxs-lookup"><span data-stu-id="dbde8-112">value</span></span>|<span data-ttu-id="dbde8-113">String</span><span class="sxs-lookup"><span data-stu-id="dbde8-113">String</span></span>| <span data-ttu-id="dbde8-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="dbde8-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="dbde8-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dbde8-115">JSON representation</span></span>

<span data-ttu-id="dbde8-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbde8-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->