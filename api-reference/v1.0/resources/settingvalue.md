---
title: Тип ресурса settingValue
description: Параметр, представленный в виде "имя-значение".
localization_priority: Normal
ms.openlocfilehash: 3edf5bdc1fae77702206eae78d53fcf0fdc5b644
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549687"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="c9769-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="c9769-103">settingValue resource type</span></span>

<span data-ttu-id="c9769-104">Параметр, представленный в виде "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="c9769-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="c9769-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9769-105">Properties</span></span>

| <span data-ttu-id="c9769-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9769-106">Property</span></span> | <span data-ttu-id="c9769-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c9769-107">Type</span></span> | <span data-ttu-id="c9769-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c9769-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c9769-109">name</span><span class="sxs-lookup"><span data-stu-id="c9769-109">name</span></span>|<span data-ttu-id="c9769-110">String</span><span class="sxs-lookup"><span data-stu-id="c9769-110">String</span></span>| <span data-ttu-id="c9769-111">Имя параметра (как определено в [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="c9769-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="c9769-112">value</span><span class="sxs-lookup"><span data-stu-id="c9769-112">value</span></span>|<span data-ttu-id="c9769-113">String</span><span class="sxs-lookup"><span data-stu-id="c9769-113">String</span></span>| <span data-ttu-id="c9769-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="c9769-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="c9769-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c9769-115">JSON representation</span></span>

<span data-ttu-id="c9769-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9769-116">Here is a JSON representation of the resource.</span></span>

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
