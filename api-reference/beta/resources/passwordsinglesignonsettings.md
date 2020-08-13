---
title: Тип ресурса Пассвордсинглесигнонсеттингс
description: Параметры, связанные с единым входом на основе паролей
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4da86cb39a1b16c9312ebe8de35c7fc87a09fdb
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658189"
---
# <a name="passwordsinglesignonsettings-resource-type"></a><span data-ttu-id="4deb7-103">Тип ресурса Пассвордсинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="4deb7-103">passwordSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4deb7-104">Содержит коллекцию параметров единого входа на основе паролей.</span><span class="sxs-lookup"><span data-stu-id="4deb7-104">Contains the collection of Password-based single sign-on settings.</span></span>

## <a name="properties"></a><span data-ttu-id="4deb7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4deb7-105">Properties</span></span>

| <span data-ttu-id="4deb7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4deb7-106">Property</span></span>     | <span data-ttu-id="4deb7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4deb7-107">Type</span></span>        | <span data-ttu-id="4deb7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4deb7-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4deb7-109">fields</span><span class="sxs-lookup"><span data-stu-id="4deb7-109">fields</span></span>|<span data-ttu-id="4deb7-110">Коллекция [пассвордсинглесигнонфиелд](passwordsinglesignonfield.md)</span><span class="sxs-lookup"><span data-stu-id="4deb7-110">[passwordSingleSignOnField](passwordsinglesignonfield.md) collection</span></span>||

## <a name="json-representation"></a><span data-ttu-id="4deb7-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4deb7-111">JSON representation</span></span>

<span data-ttu-id="4deb7-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4deb7-112">The following is a JSON representation of the resource.</span></span>

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