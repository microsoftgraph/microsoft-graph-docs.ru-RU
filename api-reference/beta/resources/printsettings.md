---
title: Тип ресурса Принтсеттингс
description: Представляет параметры на уровне клиента для универсальной службы печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 01c98eb68031018e6f7a32837e49a2095c7880d2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521238"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="b5e5c-103">Тип ресурса Принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="b5e5c-103">printSettings resource type</span></span>

<span data-ttu-id="b5e5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5e5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e5c-105">Представляет параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="b5e5c-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="b5e5c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5e5c-106">Properties</span></span>
| <span data-ttu-id="b5e5c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5e5c-107">Property</span></span>     | <span data-ttu-id="b5e5c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b5e5c-108">Type</span></span>        | <span data-ttu-id="b5e5c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b5e5c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5e5c-110">документконверсионенаблед</span><span class="sxs-lookup"><span data-stu-id="b5e5c-110">documentConversionEnabled</span></span>|<span data-ttu-id="b5e5c-111">Логический</span><span class="sxs-lookup"><span data-stu-id="b5e5c-111">Boolean</span></span>|<span data-ttu-id="b5e5c-112">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5e5c-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="b5e5c-113">Если включено преобразование документов, то при необходимости в универсальной службе печати документы автоматически преобразуются в формат, совместимый с принтером (XPS — PDF).</span><span class="sxs-lookup"><span data-stu-id="b5e5c-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5e5c-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5e5c-114">JSON representation</span></span>

<span data-ttu-id="b5e5c-115">Ниже представлено представление объекта Принтсеттингс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5e5c-115">The following is a JSON representation of printSettings.</span></span>
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


