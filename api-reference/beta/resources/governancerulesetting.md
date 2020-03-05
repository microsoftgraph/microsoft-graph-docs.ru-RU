---
title: Тип ресурса Говернанцерулесеттинг
description: Представляет правила, из которых состоят параметры ролей.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 32be4465ffcd710bbfdaf8f3c60b3813a0b7d3be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497323"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="89d59-103">Тип ресурса Говернанцерулесеттинг</span><span class="sxs-lookup"><span data-stu-id="89d59-103">governanceRuleSetting resource type</span></span>

<span data-ttu-id="89d59-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="89d59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89d59-105">Представляет правила, из которых состоят параметры ролей.</span><span class="sxs-lookup"><span data-stu-id="89d59-105">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="89d59-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="89d59-106">Properties</span></span>
|<span data-ttu-id="89d59-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="89d59-107">Property</span></span>      | <span data-ttu-id="89d59-108">Тип</span><span class="sxs-lookup"><span data-stu-id="89d59-108">Type</span></span>         |<span data-ttu-id="89d59-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89d59-109">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="89d59-110">рулеидентифиер</span><span class="sxs-lookup"><span data-stu-id="89d59-110">ruleIdentifier</span></span>|<span data-ttu-id="89d59-111">String</span><span class="sxs-lookup"><span data-stu-id="89d59-111">String</span></span>        |<span data-ttu-id="89d59-112">Идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="89d59-112">The id of the rule.</span></span> <span data-ttu-id="89d59-113">Например, ``ExpirationRule`` и ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="89d59-113">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="89d59-114">setting</span><span class="sxs-lookup"><span data-stu-id="89d59-114">setting</span></span>       |<span data-ttu-id="89d59-115">String</span><span class="sxs-lookup"><span data-stu-id="89d59-115">String</span></span>        |<span data-ttu-id="89d59-116">Параметры правила.</span><span class="sxs-lookup"><span data-stu-id="89d59-116">The settings of the rule.</span></span> <span data-ttu-id="89d59-117">Значением является строка JSON со списком пар в формате Parameter_Name: Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="89d59-117">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="89d59-118">Пример: `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="89d59-118">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89d59-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89d59-119">JSON representation</span></span>

<span data-ttu-id="89d59-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89d59-120">Here is a JSON representation of the resource.</span></span>

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
