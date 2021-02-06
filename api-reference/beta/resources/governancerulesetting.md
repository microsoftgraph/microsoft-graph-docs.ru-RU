---
title: Тип ресурса governanceRuleSetting
description: Представляет правила, из которого состоят параметры роли.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: b55ddfea8f46f9d064b4a032a804c2c5f4847d1a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132694"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="f3d28-103">Тип ресурса governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="f3d28-103">governanceRuleSetting resource type</span></span>

<span data-ttu-id="f3d28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3d28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3d28-105">Представляет правила, из которого состоят параметры роли.</span><span class="sxs-lookup"><span data-stu-id="f3d28-105">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="f3d28-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3d28-106">Properties</span></span>
|<span data-ttu-id="f3d28-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3d28-107">Property</span></span>      | <span data-ttu-id="f3d28-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f3d28-108">Type</span></span>         |<span data-ttu-id="f3d28-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f3d28-109">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="f3d28-110">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3d28-110">ruleIdentifier</span></span>|<span data-ttu-id="f3d28-111">Строка</span><span class="sxs-lookup"><span data-stu-id="f3d28-111">String</span></span>        |<span data-ttu-id="f3d28-112">ИД правила.</span><span class="sxs-lookup"><span data-stu-id="f3d28-112">The id of the rule.</span></span> <span data-ttu-id="f3d28-113">Например, ``ExpirationRule`` и ``MfaRule`` .</span><span class="sxs-lookup"><span data-stu-id="f3d28-113">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="f3d28-114">setting</span><span class="sxs-lookup"><span data-stu-id="f3d28-114">setting</span></span>       |<span data-ttu-id="f3d28-115">String</span><span class="sxs-lookup"><span data-stu-id="f3d28-115">String</span></span>        |<span data-ttu-id="f3d28-116">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="f3d28-116">The settings of the rule.</span></span> <span data-ttu-id="f3d28-117">Значением является строка JSON со списком пар в формате Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="f3d28-117">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="f3d28-118">Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="f3d28-118">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3d28-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f3d28-119">JSON representation</span></span>

<span data-ttu-id="f3d28-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3d28-120">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


