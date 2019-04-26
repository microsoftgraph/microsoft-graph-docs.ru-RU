---
title: Тип ресурса Едукатионксвдатапровидер
description: 'Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4dbbf5d5791df1035fcd9fe1a953d8a9a347070a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340587"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="f2b09-103">Тип ресурса Едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="f2b09-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2b09-104">Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.</span><span class="sxs-lookup"><span data-stu-id="f2b09-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="f2b09-105">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="f2b09-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f2b09-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2b09-106">Properties</span></span>

| <span data-ttu-id="f2b09-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2b09-107">Property</span></span> | <span data-ttu-id="f2b09-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f2b09-108">Type</span></span> | <span data-ttu-id="f2b09-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f2b09-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f2b09-110">**настроек**</span><span class="sxs-lookup"><span data-stu-id="f2b09-110">**customizations**</span></span> | [<span data-ttu-id="f2b09-111">Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="f2b09-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="f2b09-112">НеОбязательные настройки, которые необходимо применить к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f2b09-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2b09-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2b09-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
