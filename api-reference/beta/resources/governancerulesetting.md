---
title: Тип ресурса governanceRuleSetting
description: Представляет правила, которые предоставляют параметры роли.
ms.openlocfilehash: 486b5163c59772c971cfc1d61a98817b7f0c16f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079012"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="29e65-103">Тип ресурса governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="29e65-103">governanceRuleSetting resource type</span></span>

> <span data-ttu-id="29e65-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29e65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29e65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29e65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29e65-106">Представляет правила, которые предоставляют параметры роли.</span><span class="sxs-lookup"><span data-stu-id="29e65-106">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="29e65-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="29e65-107">Properties</span></span>
|<span data-ttu-id="29e65-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="29e65-108">Property</span></span>      | <span data-ttu-id="29e65-109">Тип</span><span class="sxs-lookup"><span data-stu-id="29e65-109">Type</span></span>         |<span data-ttu-id="29e65-110">Description</span><span class="sxs-lookup"><span data-stu-id="29e65-110">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="29e65-111">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="29e65-111">ruleIdentifier</span></span>|<span data-ttu-id="29e65-112">String</span><span class="sxs-lookup"><span data-stu-id="29e65-112">String</span></span>        |<span data-ttu-id="29e65-113">Идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="29e65-113">The id of the rule.</span></span> <span data-ttu-id="29e65-114">Например ``ExpirationRule`` и ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="29e65-114">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="29e65-115">setting</span><span class="sxs-lookup"><span data-stu-id="29e65-115">setting</span></span>       |<span data-ttu-id="29e65-116">String</span><span class="sxs-lookup"><span data-stu-id="29e65-116">String</span></span>        |<span data-ttu-id="29e65-117">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="29e65-117">The settings of the rule.</span></span> <span data-ttu-id="29e65-118">Значение — это строка JSON со списком пар в формате Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="29e65-118">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="29e65-119">Например, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="29e65-119">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29e65-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29e65-120">JSON representation</span></span>

<span data-ttu-id="29e65-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29e65-121">Here is a JSON representation of the resource.</span></span>

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