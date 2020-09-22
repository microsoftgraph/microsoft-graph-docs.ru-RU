---
title: Тип ресурса Персистентбровсерсессионконтрол
description: Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad25e798b2f49ab373c85ee9072b3e7990cfe67d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984231"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="6c91e-103">Тип ресурса Персистентбровсерсессионконтрол</span><span class="sxs-lookup"><span data-stu-id="6c91e-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="6c91e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c91e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c91e-105">Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="6c91e-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="6c91e-106">Наследуется от [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="6c91e-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6c91e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c91e-107">Properties</span></span>

| <span data-ttu-id="6c91e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c91e-108">Property</span></span>     | <span data-ttu-id="6c91e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6c91e-109">Type</span></span>        | <span data-ttu-id="6c91e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6c91e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c91e-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6c91e-111">isEnabled</span></span>     |<span data-ttu-id="6c91e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c91e-112">Boolean</span></span>      | <span data-ttu-id="6c91e-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="6c91e-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="6c91e-114">mode</span><span class="sxs-lookup"><span data-stu-id="6c91e-114">mode</span></span>|<span data-ttu-id="6c91e-115">String</span><span class="sxs-lookup"><span data-stu-id="6c91e-115">String</span></span>| <span data-ttu-id="6c91e-116">Возможные значения: `always`, `never`.</span><span class="sxs-lookup"><span data-stu-id="6c91e-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c91e-117">Связи</span><span class="sxs-lookup"><span data-stu-id="6c91e-117">Relationships</span></span>

<span data-ttu-id="6c91e-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6c91e-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c91e-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6c91e-119">JSON representation</span></span>

<span data-ttu-id="6c91e-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c91e-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "mode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persistentBrowserSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

