---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
ms.openlocfilehash: 433fc0d3ab3a524b86bbf1fc46dbe5185549473b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333732"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="d773e-103">Тип ресурса Говернанцерулесеттинг</span><span class="sxs-lookup"><span data-stu-id="d773e-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d773e-104">Представляет правила, из которых состоят параметры ролей.</span><span class="sxs-lookup"><span data-stu-id="d773e-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="d773e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d773e-105">Properties</span></span>
|<span data-ttu-id="d773e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d773e-106">Property</span></span>      | <span data-ttu-id="d773e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d773e-107">Type</span></span>         |<span data-ttu-id="d773e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d773e-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="d773e-109">Рулеидентифиер</span><span class="sxs-lookup"><span data-stu-id="d773e-109">ruleIdentifier</span></span>|<span data-ttu-id="d773e-110">String</span><span class="sxs-lookup"><span data-stu-id="d773e-110">String</span></span>        |<span data-ttu-id="d773e-111">Идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="d773e-111">The id of the rule.</span></span> <span data-ttu-id="d773e-112">Например, ``ExpirationRule`` и ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="d773e-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="d773e-113">setting</span><span class="sxs-lookup"><span data-stu-id="d773e-113">setting</span></span>       |<span data-ttu-id="d773e-114">String</span><span class="sxs-lookup"><span data-stu-id="d773e-114">String</span></span>        |<span data-ttu-id="d773e-115">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="d773e-115">The settings of the rule.</span></span> <span data-ttu-id="d773e-116">Значением является строка JSON со списком пар в формате Параметер_наме: Параметер_валуе.</span><span class="sxs-lookup"><span data-stu-id="d773e-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="d773e-117">Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="d773e-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d773e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d773e-118">JSON representation</span></span>

<span data-ttu-id="d773e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d773e-119">Here is a JSON representation of the resource.</span></span>

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
