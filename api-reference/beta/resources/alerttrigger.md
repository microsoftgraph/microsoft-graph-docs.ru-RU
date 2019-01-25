---
title: Тип ресурса alertTrigger
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: cda1dde9b22b9304fd412405758435be2f6143bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516317"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="4d8c4-104">Тип ресурса alertTrigger</span><span class="sxs-lookup"><span data-stu-id="4d8c4-104">alertTrigger resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d8c4-105">Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).</span><span class="sxs-lookup"><span data-stu-id="4d8c4-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="4d8c4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d8c4-106">Properties</span></span>

| <span data-ttu-id="4d8c4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d8c4-107">Property</span></span>   | <span data-ttu-id="4d8c4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4d8c4-108">Type</span></span>|<span data-ttu-id="4d8c4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4d8c4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d8c4-110">name</span><span class="sxs-lookup"><span data-stu-id="4d8c4-110">name</span></span>|<span data-ttu-id="4d8c4-111">String</span><span class="sxs-lookup"><span data-stu-id="4d8c4-111">String</span></span>|<span data-ttu-id="4d8c4-112">Имя свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="4d8c4-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="4d8c4-113">type</span><span class="sxs-lookup"><span data-stu-id="4d8c4-113">type</span></span>|<span data-ttu-id="4d8c4-114">String</span><span class="sxs-lookup"><span data-stu-id="4d8c4-114">String</span></span>|<span data-ttu-id="4d8c4-115">Тип свойства в пары "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="4d8c4-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="4d8c4-116">Например String, Boolean, и т.д.</span><span class="sxs-lookup"><span data-stu-id="4d8c4-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="4d8c4-117">value</span><span class="sxs-lookup"><span data-stu-id="4d8c4-117">value</span></span>|<span data-ttu-id="4d8c4-118">String</span><span class="sxs-lookup"><span data-stu-id="4d8c4-118">String</span></span>|<span data-ttu-id="4d8c4-119">Значение свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="4d8c4-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d8c4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d8c4-120">JSON representation</span></span>

<span data-ttu-id="4d8c4-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d8c4-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="4d8c4-122">Пример</span><span class="sxs-lookup"><span data-stu-id="4d8c4-122">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/alerttrigger.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
