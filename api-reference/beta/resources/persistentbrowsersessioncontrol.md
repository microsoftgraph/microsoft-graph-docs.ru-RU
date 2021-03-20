---
title: тип ресурса persistentBrowserSessionControl
description: Управление сеансом, чтобы определить, следует ли сохранять файлы cookie или нет.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4ef2abb60c364969e4bb9f739e45ae537162188f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952776"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="86916-103">тип ресурса persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="86916-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="86916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86916-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86916-105">Управление сеансом, чтобы определить, следует ли сохранять файлы cookie или нет.</span><span class="sxs-lookup"><span data-stu-id="86916-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="86916-106">Наследуется от [управления сеансами условного доступа.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="86916-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="86916-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86916-107">Properties</span></span>

| <span data-ttu-id="86916-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86916-108">Property</span></span>     | <span data-ttu-id="86916-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86916-109">Type</span></span>        | <span data-ttu-id="86916-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86916-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86916-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="86916-111">isEnabled</span></span>     |<span data-ttu-id="86916-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="86916-112">Boolean</span></span>      | <span data-ttu-id="86916-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="86916-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="86916-114">mode</span><span class="sxs-lookup"><span data-stu-id="86916-114">mode</span></span>|<span data-ttu-id="86916-115">persistentBrowserSessionMode</span><span class="sxs-lookup"><span data-stu-id="86916-115">persistentBrowserSessionMode</span></span>| <span data-ttu-id="86916-116">Возможные значения: `always`, `never`.</span><span class="sxs-lookup"><span data-stu-id="86916-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86916-117">Связи</span><span class="sxs-lookup"><span data-stu-id="86916-117">Relationships</span></span>

<span data-ttu-id="86916-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="86916-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="86916-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="86916-119">JSON representation</span></span>

<span data-ttu-id="86916-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86916-120">The following is a JSON representation of the resource.</span></span>

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

