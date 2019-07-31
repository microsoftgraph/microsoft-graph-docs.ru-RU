---
title: Тип ресурса Едукатионксвдатапровидер
description: 'Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f515744f5206ea132531373e3df317e02dd6cbb4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006404"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="362c1-103">Тип ресурса Едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="362c1-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="362c1-104">Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.</span><span class="sxs-lookup"><span data-stu-id="362c1-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="362c1-105">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="362c1-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="362c1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="362c1-106">Properties</span></span>

| <span data-ttu-id="362c1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="362c1-107">Property</span></span> | <span data-ttu-id="362c1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="362c1-108">Type</span></span> | <span data-ttu-id="362c1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="362c1-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="362c1-110">**настроек**</span><span class="sxs-lookup"><span data-stu-id="362c1-110">**customizations**</span></span> | [<span data-ttu-id="362c1-111">Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="362c1-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="362c1-112">Необязательные настройки, которые необходимо применить к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="362c1-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="362c1-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="362c1-113">JSON representation</span></span>

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
