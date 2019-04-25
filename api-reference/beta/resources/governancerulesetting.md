---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547461"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="639d7-103">Тип ресурса Говернанцерулесеттинг</span><span class="sxs-lookup"><span data-stu-id="639d7-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="639d7-104">Представляет правила, из которых состоят параметры ролей.</span><span class="sxs-lookup"><span data-stu-id="639d7-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="639d7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="639d7-105">Properties</span></span>
|<span data-ttu-id="639d7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="639d7-106">Property</span></span>      | <span data-ttu-id="639d7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="639d7-107">Type</span></span>         |<span data-ttu-id="639d7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="639d7-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="639d7-109">Рулеидентифиер</span><span class="sxs-lookup"><span data-stu-id="639d7-109">ruleIdentifier</span></span>|<span data-ttu-id="639d7-110">String</span><span class="sxs-lookup"><span data-stu-id="639d7-110">String</span></span>        |<span data-ttu-id="639d7-111">Идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="639d7-111">The id of the rule.</span></span> <span data-ttu-id="639d7-112">Например, ``ExpirationRule`` и ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="639d7-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="639d7-113">setting</span><span class="sxs-lookup"><span data-stu-id="639d7-113">setting</span></span>       |<span data-ttu-id="639d7-114">String</span><span class="sxs-lookup"><span data-stu-id="639d7-114">String</span></span>        |<span data-ttu-id="639d7-115">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="639d7-115">The settings of the rule.</span></span> <span data-ttu-id="639d7-116">Значением является строка JSON со списком пар в формате Параметер_наме: Параметер_валуе.</span><span class="sxs-lookup"><span data-stu-id="639d7-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="639d7-117">Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="639d7-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="639d7-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="639d7-118">JSON representation</span></span>

<span data-ttu-id="639d7-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="639d7-119">Here is a JSON representation of the resource.</span></span>

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
