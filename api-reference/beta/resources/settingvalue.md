---
title: Тип ресурса settingValue
description: Параметр, представленный парой "имя-значение".
ms.openlocfilehash: fb1c249fba9506b2a4c6ad29d04f98b36c82f53f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080198"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="701f7-103">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="701f7-103">settingValue resource type</span></span>

> <span data-ttu-id="701f7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="701f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="701f7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="701f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="701f7-106">Параметр, представленный парой "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="701f7-106">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="701f7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="701f7-107">Properties</span></span>
| <span data-ttu-id="701f7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="701f7-108">Property</span></span>     | <span data-ttu-id="701f7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="701f7-109">Type</span></span>   |<span data-ttu-id="701f7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="701f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="701f7-111">name</span><span class="sxs-lookup"><span data-stu-id="701f7-111">name</span></span>|<span data-ttu-id="701f7-112">строка</span><span class="sxs-lookup"><span data-stu-id="701f7-112">string</span></span>|<span data-ttu-id="701f7-113">Имя удаляемого параметра (как определено directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="701f7-113">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="701f7-114">value</span><span class="sxs-lookup"><span data-stu-id="701f7-114">value</span></span>|<span data-ttu-id="701f7-115">строка</span><span class="sxs-lookup"><span data-stu-id="701f7-115">string</span></span>|<span data-ttu-id="701f7-116">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="701f7-116">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="701f7-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="701f7-117">JSON representation</span></span>

<span data-ttu-id="701f7-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="701f7-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
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
