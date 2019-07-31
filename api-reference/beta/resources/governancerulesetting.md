---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bfc3bb7895a3ec66a32456b48901fc456d3c3b2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971874"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="ab51a-103">Тип ресурса Говернанцерулесеттинг</span><span class="sxs-lookup"><span data-stu-id="ab51a-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab51a-104">Представляет правила, из которых состоят параметры ролей.</span><span class="sxs-lookup"><span data-stu-id="ab51a-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="ab51a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab51a-105">Properties</span></span>
|<span data-ttu-id="ab51a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab51a-106">Property</span></span>      | <span data-ttu-id="ab51a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ab51a-107">Type</span></span>         |<span data-ttu-id="ab51a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ab51a-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="ab51a-109">Рулеидентифиер</span><span class="sxs-lookup"><span data-stu-id="ab51a-109">ruleIdentifier</span></span>|<span data-ttu-id="ab51a-110">String</span><span class="sxs-lookup"><span data-stu-id="ab51a-110">String</span></span>        |<span data-ttu-id="ab51a-111">Идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="ab51a-111">The id of the rule.</span></span> <span data-ttu-id="ab51a-112">Например, ``ExpirationRule`` и ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="ab51a-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="ab51a-113">setting</span><span class="sxs-lookup"><span data-stu-id="ab51a-113">setting</span></span>       |<span data-ttu-id="ab51a-114">String</span><span class="sxs-lookup"><span data-stu-id="ab51a-114">String</span></span>        |<span data-ttu-id="ab51a-115">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="ab51a-115">The settings of the rule.</span></span> <span data-ttu-id="ab51a-116">Значением является строка JSON со списком пар в формате Параметер_наме: Параметер_валуе.</span><span class="sxs-lookup"><span data-stu-id="ab51a-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="ab51a-117">Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="ab51a-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab51a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab51a-118">JSON representation</span></span>

<span data-ttu-id="ab51a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab51a-119">Here is a JSON representation of the resource.</span></span>

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
