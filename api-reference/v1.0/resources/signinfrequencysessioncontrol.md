---
title: Тип ресурса signInFrequencySessionControl
description: Управление сеансом для принудительной регистрации.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4a89a9337bc032210873de3ceb05949f935693f1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137125"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="997ba-103">Тип ресурса signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="997ba-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="997ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="997ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="997ba-105">Управление сеансом для принудительной частоты входов.</span><span class="sxs-lookup"><span data-stu-id="997ba-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="997ba-106">Наследуется от [контроля сеанса условного доступа.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="997ba-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="997ba-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="997ba-107">Properties</span></span>

| <span data-ttu-id="997ba-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="997ba-108">Property</span></span>     | <span data-ttu-id="997ba-109">Тип</span><span class="sxs-lookup"><span data-stu-id="997ba-109">Type</span></span>        | <span data-ttu-id="997ba-110">Описание</span><span class="sxs-lookup"><span data-stu-id="997ba-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="997ba-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="997ba-111">isEnabled</span></span>     |<span data-ttu-id="997ba-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="997ba-112">Boolean</span></span>      | <span data-ttu-id="997ba-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="997ba-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="997ba-114">type</span><span class="sxs-lookup"><span data-stu-id="997ba-114">type</span></span>          |<span data-ttu-id="997ba-115">String</span><span class="sxs-lookup"><span data-stu-id="997ba-115">String</span></span>       | <span data-ttu-id="997ba-116">Возможные значения: `days`, `hours`.</span><span class="sxs-lookup"><span data-stu-id="997ba-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="997ba-117">value</span><span class="sxs-lookup"><span data-stu-id="997ba-117">value</span></span>         |<span data-ttu-id="997ba-118">Int32</span><span class="sxs-lookup"><span data-stu-id="997ba-118">Int32</span></span>        | <span data-ttu-id="997ba-119">Количество или `days` `hours` .</span><span class="sxs-lookup"><span data-stu-id="997ba-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="997ba-120">Связи</span><span class="sxs-lookup"><span data-stu-id="997ba-120">Relationships</span></span>

<span data-ttu-id="997ba-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="997ba-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="997ba-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="997ba-122">JSON representation</span></span>

<span data-ttu-id="997ba-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="997ba-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "type": "String",
  "value": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

