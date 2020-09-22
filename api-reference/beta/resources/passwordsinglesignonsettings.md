---
title: Тип ресурса Пассвордсинглесигнонсеттингс
description: Параметры, связанные с единым входом на основе паролей
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a1b2739ecbd5d09358e58203ab61d4e65c48716b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998175"
---
# <a name="passwordsinglesignonsettings-resource-type"></a><span data-ttu-id="e3aaa-103">Тип ресурса Пассвордсинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="e3aaa-103">passwordSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3aaa-104">Содержит коллекцию параметров единого входа на основе паролей.</span><span class="sxs-lookup"><span data-stu-id="e3aaa-104">Contains the collection of Password-based single sign-on settings.</span></span>

## <a name="properties"></a><span data-ttu-id="e3aaa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3aaa-105">Properties</span></span>

| <span data-ttu-id="e3aaa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3aaa-106">Property</span></span>     | <span data-ttu-id="e3aaa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e3aaa-107">Type</span></span>        | <span data-ttu-id="e3aaa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e3aaa-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3aaa-109">fields</span><span class="sxs-lookup"><span data-stu-id="e3aaa-109">fields</span></span>|<span data-ttu-id="e3aaa-110">Коллекция [пассвордсинглесигнонфиелд](passwordsinglesignonfield.md)</span><span class="sxs-lookup"><span data-stu-id="e3aaa-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) collection</span></span>||

## <a name="json-representation"></a><span data-ttu-id="e3aaa-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3aaa-111">JSON representation</span></span>

<span data-ttu-id="e3aaa-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3aaa-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnSettings",
  "baseType": null
}-->

```json
{
  "fields": [{"@odata.type": "microsoft.graph.passwordSingleSignOnField"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

