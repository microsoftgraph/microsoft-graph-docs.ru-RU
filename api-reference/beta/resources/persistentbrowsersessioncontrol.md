---
title: Тип ресурса Персистентбровсерсессионконтрол
description: Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d8924c442cc4795c5f7e51d26826ad6ee2b7f0f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998070"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="09a94-103">Тип ресурса Персистентбровсерсессионконтрол</span><span class="sxs-lookup"><span data-stu-id="09a94-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="09a94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09a94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09a94-105">Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="09a94-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="09a94-106">Наследуется от [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="09a94-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="09a94-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="09a94-107">Properties</span></span>

| <span data-ttu-id="09a94-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="09a94-108">Property</span></span>     | <span data-ttu-id="09a94-109">Тип</span><span class="sxs-lookup"><span data-stu-id="09a94-109">Type</span></span>        | <span data-ttu-id="09a94-110">Описание</span><span class="sxs-lookup"><span data-stu-id="09a94-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09a94-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="09a94-111">isEnabled</span></span>     |<span data-ttu-id="09a94-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a94-112">Boolean</span></span>      | <span data-ttu-id="09a94-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="09a94-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="09a94-114">mode</span><span class="sxs-lookup"><span data-stu-id="09a94-114">mode</span></span>|<span data-ttu-id="09a94-115">String</span><span class="sxs-lookup"><span data-stu-id="09a94-115">String</span></span>| <span data-ttu-id="09a94-116">Возможные значения: `always`, `never`.</span><span class="sxs-lookup"><span data-stu-id="09a94-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09a94-117">Связи</span><span class="sxs-lookup"><span data-stu-id="09a94-117">Relationships</span></span>

<span data-ttu-id="09a94-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="09a94-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09a94-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="09a94-119">JSON representation</span></span>

<span data-ttu-id="09a94-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09a94-120">The following is a JSON representation of the resource.</span></span>

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

