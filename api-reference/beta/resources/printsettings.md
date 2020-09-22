---
title: Тип ресурса Принтсеттингс
description: Представляет параметры на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c9af888d85256b88d4212cc84ba74d8dcdd5b590
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973822"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="255a1-103">Тип ресурса Принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="255a1-103">printSettings resource type</span></span>

<span data-ttu-id="255a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="255a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="255a1-105">Представляет параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="255a1-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="255a1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="255a1-106">Properties</span></span>
| <span data-ttu-id="255a1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="255a1-107">Property</span></span>     | <span data-ttu-id="255a1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="255a1-108">Type</span></span>        | <span data-ttu-id="255a1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="255a1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="255a1-110">документконверсионенаблед</span><span class="sxs-lookup"><span data-stu-id="255a1-110">documentConversionEnabled</span></span>|<span data-ttu-id="255a1-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="255a1-111">Boolean</span></span>|<span data-ttu-id="255a1-112">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="255a1-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="255a1-113">Если включено преобразование документов, то при необходимости в универсальной службе печати документы автоматически преобразуются в формат, совместимый с принтером (XPS — PDF).</span><span class="sxs-lookup"><span data-stu-id="255a1-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="255a1-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="255a1-114">JSON representation</span></span>

<span data-ttu-id="255a1-115">Ниже представлено представление объекта Принтсеттингс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="255a1-115">The following is a JSON representation of printSettings.</span></span>
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


