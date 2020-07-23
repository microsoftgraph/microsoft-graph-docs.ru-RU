---
title: Тип ресурса Персистентбровсерсессионконтрол
description: Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a747f2d51d43b30da7dd7566a767cfb5f8c3fcd5
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384886"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="cebbf-103">Тип ресурса Персистентбровсерсессионконтрол</span><span class="sxs-lookup"><span data-stu-id="cebbf-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="cebbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cebbf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cebbf-105">Элемент управления сеансом, чтобы определить, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="cebbf-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="cebbf-106">Наследуется от [управления сеансом условного доступа](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="cebbf-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cebbf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cebbf-107">Properties</span></span>

| <span data-ttu-id="cebbf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cebbf-108">Property</span></span>     | <span data-ttu-id="cebbf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cebbf-109">Type</span></span>        | <span data-ttu-id="cebbf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cebbf-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cebbf-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cebbf-111">isEnabled</span></span>     |<span data-ttu-id="cebbf-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="cebbf-112">Boolean</span></span>      | <span data-ttu-id="cebbf-113">Указывает, включен ли элемент управления сеансом.</span><span class="sxs-lookup"><span data-stu-id="cebbf-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="cebbf-114">mode</span><span class="sxs-lookup"><span data-stu-id="cebbf-114">mode</span></span>|<span data-ttu-id="cebbf-115">String</span><span class="sxs-lookup"><span data-stu-id="cebbf-115">String</span></span>| <span data-ttu-id="cebbf-116">Возможные значения: `always`, `never`.</span><span class="sxs-lookup"><span data-stu-id="cebbf-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cebbf-117">Связи</span><span class="sxs-lookup"><span data-stu-id="cebbf-117">Relationships</span></span>

<span data-ttu-id="cebbf-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cebbf-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cebbf-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cebbf-119">JSON representation</span></span>

<span data-ttu-id="cebbf-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cebbf-120">The following is a JSON representation of the resource.</span></span>

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
