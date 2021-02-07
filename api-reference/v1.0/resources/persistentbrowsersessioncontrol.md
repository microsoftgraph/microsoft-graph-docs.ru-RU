---
title: Тип ресурса persistentBrowserSessionControl
description: Управление сеансом для определения того, следует ли сохранять файлы cookie.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7b418f16a69e5b97cbb42bc81994dfd87e5a3c1e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135739"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="78754-103">Тип ресурса persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="78754-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="78754-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78754-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78754-105">Управление сеансом для определения того, следует ли сохранять файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="78754-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="78754-106">Наследуется от [контроля сеанса условного доступа.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="78754-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="78754-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="78754-107">Properties</span></span>

| <span data-ttu-id="78754-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="78754-108">Property</span></span>     | <span data-ttu-id="78754-109">Тип</span><span class="sxs-lookup"><span data-stu-id="78754-109">Type</span></span>        | <span data-ttu-id="78754-110">Описание</span><span class="sxs-lookup"><span data-stu-id="78754-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78754-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="78754-111">isEnabled</span></span>     |<span data-ttu-id="78754-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="78754-112">Boolean</span></span>      | <span data-ttu-id="78754-113">Указывает, включено ли управление сеансом.</span><span class="sxs-lookup"><span data-stu-id="78754-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="78754-114">mode</span><span class="sxs-lookup"><span data-stu-id="78754-114">mode</span></span>|<span data-ttu-id="78754-115">String</span><span class="sxs-lookup"><span data-stu-id="78754-115">String</span></span>| <span data-ttu-id="78754-116">Возможные значения: `always`, `never`.</span><span class="sxs-lookup"><span data-stu-id="78754-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78754-117">Связи</span><span class="sxs-lookup"><span data-stu-id="78754-117">Relationships</span></span>

<span data-ttu-id="78754-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="78754-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78754-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="78754-119">JSON representation</span></span>

<span data-ttu-id="78754-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78754-120">The following is a JSON representation of the resource.</span></span>

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

