---
title: Тип ресурса governanceRuleSetting
description: Представляет правила, которые предоставляют параметры роли.
localization_priority: Normal
ms.openlocfilehash: 7554c96daec70a95cde5ab0c3faedfba74764cff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894259"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="eecad-103">Тип ресурса governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="eecad-103">governanceRuleSetting resource type</span></span>

> <span data-ttu-id="eecad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eecad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eecad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eecad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eecad-106">Представляет правила, которые предоставляют параметры роли.</span><span class="sxs-lookup"><span data-stu-id="eecad-106">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="eecad-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eecad-107">Properties</span></span>
|<span data-ttu-id="eecad-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eecad-108">Property</span></span>      | <span data-ttu-id="eecad-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eecad-109">Type</span></span>         |<span data-ttu-id="eecad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eecad-110">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="eecad-111">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="eecad-111">ruleIdentifier</span></span>|<span data-ttu-id="eecad-112">Строка</span><span class="sxs-lookup"><span data-stu-id="eecad-112">String</span></span>        |<span data-ttu-id="eecad-113">Идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="eecad-113">The id of the rule.</span></span> <span data-ttu-id="eecad-114">Например ``ExpirationRule`` и ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="eecad-114">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="eecad-115">setting</span><span class="sxs-lookup"><span data-stu-id="eecad-115">setting</span></span>       |<span data-ttu-id="eecad-116">String</span><span class="sxs-lookup"><span data-stu-id="eecad-116">String</span></span>        |<span data-ttu-id="eecad-117">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="eecad-117">The settings of the rule.</span></span> <span data-ttu-id="eecad-118">Значение — это строка JSON со списком пар в формате Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="eecad-118">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="eecad-119">Например, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="eecad-119">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eecad-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eecad-120">JSON representation</span></span>

<span data-ttu-id="eecad-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eecad-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
