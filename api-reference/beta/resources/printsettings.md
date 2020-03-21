---
title: Тип ресурса Принтсеттингс
description: Представляет параметры на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 08d8409113c9c2f480200999c47ca18c300f245f
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896059"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="216dc-103">Тип ресурса Принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="216dc-103">printSettings resource type</span></span>

<span data-ttu-id="216dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="216dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="216dc-105">Представляет параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="216dc-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="216dc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="216dc-106">Properties</span></span>
| <span data-ttu-id="216dc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="216dc-107">Property</span></span>     | <span data-ttu-id="216dc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="216dc-108">Type</span></span>        | <span data-ttu-id="216dc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="216dc-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="216dc-110">документконверсионенаблед</span><span class="sxs-lookup"><span data-stu-id="216dc-110">documentConversionEnabled</span></span>|<span data-ttu-id="216dc-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="216dc-111">Boolean</span></span>|<span data-ttu-id="216dc-112">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="216dc-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="216dc-113">Если включено преобразование документов, то при необходимости в универсальной службе печати документы автоматически преобразуются в формат, совместимый с принтером (XPS — PDF).</span><span class="sxs-lookup"><span data-stu-id="216dc-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="216dc-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="216dc-114">JSON representation</span></span>

<span data-ttu-id="216dc-115">Ниже представлено представление объекта Принтсеттингс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="216dc-115">The following is a JSON representation of printSettings.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printSettings"
}-->

```json
{
  "documentConversionEnabled": true
}

```
