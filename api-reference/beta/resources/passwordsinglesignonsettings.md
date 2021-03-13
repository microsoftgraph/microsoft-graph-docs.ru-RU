---
title: тип ресурса passwordSingleSignOnSettings
description: Параметры, связанные с одним входом на основе пароля
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3e7e4402e6416166dd7c288cdd9aa9ec5ecbba06
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761544"
---
# <a name="passwordsinglesignonsettings-resource-type"></a><span data-ttu-id="62c12-103">тип ресурса passwordSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="62c12-103">passwordSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62c12-104">Содержит коллекцию параметров единой подписи на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="62c12-104">Contains the collection of Password-based single sign-on settings.</span></span>

## <a name="properties"></a><span data-ttu-id="62c12-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="62c12-105">Properties</span></span>

| <span data-ttu-id="62c12-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="62c12-106">Property</span></span>     | <span data-ttu-id="62c12-107">Тип</span><span class="sxs-lookup"><span data-stu-id="62c12-107">Type</span></span>        | <span data-ttu-id="62c12-108">Описание</span><span class="sxs-lookup"><span data-stu-id="62c12-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62c12-109">fields</span><span class="sxs-lookup"><span data-stu-id="62c12-109">fields</span></span>|<span data-ttu-id="62c12-110">[коллекция passwordSingleSignOnField](passwordsinglesignonfield.md)</span><span class="sxs-lookup"><span data-stu-id="62c12-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) collection</span></span>||

## <a name="json-representation"></a><span data-ttu-id="62c12-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62c12-111">JSON representation</span></span>

<span data-ttu-id="62c12-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62c12-112">The following is a JSON representation of the resource.</span></span>

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

