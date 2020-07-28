---
title: Тип ресурса Едукатионксвдатапровидер
description: 'Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 33cb0268eeb8c6d6b896dfb8ab02f7bb59b00e98
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434986"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="86d3c-103">Тип ресурса Едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="86d3c-103">educationCsvDataProvider resource type</span></span>

<span data-ttu-id="86d3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86d3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86d3c-105">Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.</span><span class="sxs-lookup"><span data-stu-id="86d3c-105">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>

<span data-ttu-id="86d3c-106">Производный от [едукатионсинчронизатиондатапровидер].</span><span class="sxs-lookup"><span data-stu-id="86d3c-106">Derived from [educationSynchronizationDataProvider].</span></span>

## <a name="properties"></a><span data-ttu-id="86d3c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86d3c-107">Properties</span></span>

| <span data-ttu-id="86d3c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86d3c-108">Property</span></span>       | <span data-ttu-id="86d3c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86d3c-109">Type</span></span>                                     | <span data-ttu-id="86d3c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86d3c-110">Description</span></span>                                                           |
| :------------- | :--------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="86d3c-111">настроек</span><span class="sxs-lookup"><span data-stu-id="86d3c-111">customizations</span></span> | <span data-ttu-id="86d3c-112">[едукатионсинчронизатионкустомизатионс]</span><span class="sxs-lookup"><span data-stu-id="86d3c-112">[educationSynchronizationCustomizations]</span></span> | <span data-ttu-id="86d3c-113">Необязательные настройки, которые необходимо применить к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="86d3c-113">Optional customizations to be applied to the synchronization profile.</span></span> |

[едукатионсинчронизатиондатапровидер]: educationsynchronizationdataprovider.md
[educationsynchronizationdataprovider]: educationsynchronizationdataprovider.md
[едукатионсинчронизатионкустомизатионс]: educationsynchronizationcustomizations.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a><span data-ttu-id="86d3c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86d3c-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationCsvDataProvider",
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```
