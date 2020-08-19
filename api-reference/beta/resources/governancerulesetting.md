---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 45ae44dccba67ee0b03f1941dd27795a002e810b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809532"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="bd261-103">Тип ресурса Говернанцерулесеттинг</span><span class="sxs-lookup"><span data-stu-id="bd261-103">governanceRuleSetting resource type</span></span>

<span data-ttu-id="bd261-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd261-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd261-105">Представляет правила, из которых состоят параметры ролей.</span><span class="sxs-lookup"><span data-stu-id="bd261-105">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="bd261-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd261-106">Properties</span></span>
|<span data-ttu-id="bd261-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd261-107">Property</span></span>      | <span data-ttu-id="bd261-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bd261-108">Type</span></span>         |<span data-ttu-id="bd261-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bd261-109">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="bd261-110">рулеидентифиер</span><span class="sxs-lookup"><span data-stu-id="bd261-110">ruleIdentifier</span></span>|<span data-ttu-id="bd261-111">String</span><span class="sxs-lookup"><span data-stu-id="bd261-111">String</span></span>        |<span data-ttu-id="bd261-112">Идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="bd261-112">The id of the rule.</span></span> <span data-ttu-id="bd261-113">Например, ``ExpirationRule`` и ``MfaRule`` .</span><span class="sxs-lookup"><span data-stu-id="bd261-113">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="bd261-114">setting</span><span class="sxs-lookup"><span data-stu-id="bd261-114">setting</span></span>       |<span data-ttu-id="bd261-115">String</span><span class="sxs-lookup"><span data-stu-id="bd261-115">String</span></span>        |<span data-ttu-id="bd261-116">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="bd261-116">The settings of the rule.</span></span> <span data-ttu-id="bd261-117">Значением является строка JSON со списком пар в формате Parameter_Name: Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="bd261-117">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="bd261-118">Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="bd261-118">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd261-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bd261-119">JSON representation</span></span>

<span data-ttu-id="bd261-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd261-120">Here is a JSON representation of the resource.</span></span>

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
