---
title: Тип ресурса governanceRuleSetting
description: Представляет правила, которые предоставляют параметры роли.
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522240"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="3c22a-103">Тип ресурса governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="3c22a-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c22a-104">Представляет правила, которые предоставляют параметры роли.</span><span class="sxs-lookup"><span data-stu-id="3c22a-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="3c22a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c22a-105">Properties</span></span>
|<span data-ttu-id="3c22a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c22a-106">Property</span></span>      | <span data-ttu-id="3c22a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3c22a-107">Type</span></span>         |<span data-ttu-id="3c22a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3c22a-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="3c22a-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="3c22a-109">ruleIdentifier</span></span>|<span data-ttu-id="3c22a-110">String</span><span class="sxs-lookup"><span data-stu-id="3c22a-110">String</span></span>        |<span data-ttu-id="3c22a-111">Идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="3c22a-111">The id of the rule.</span></span> <span data-ttu-id="3c22a-112">Например ``ExpirationRule`` и ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="3c22a-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="3c22a-113">setting</span><span class="sxs-lookup"><span data-stu-id="3c22a-113">setting</span></span>       |<span data-ttu-id="3c22a-114">String</span><span class="sxs-lookup"><span data-stu-id="3c22a-114">String</span></span>        |<span data-ttu-id="3c22a-115">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="3c22a-115">The settings of the rule.</span></span> <span data-ttu-id="3c22a-116">Значение — это строка JSON со списком пар в формате Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="3c22a-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="3c22a-117">Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="3c22a-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c22a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c22a-118">JSON representation</span></span>

<span data-ttu-id="3c22a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c22a-119">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerulesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
