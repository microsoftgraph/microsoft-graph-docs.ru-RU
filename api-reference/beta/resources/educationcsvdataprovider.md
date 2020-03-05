---
title: Тип ресурса Едукатионксвдатапровидер
description: 'Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 207fee7f889c4369862918943371e2d629c8fab9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502174"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="96663-103">Тип ресурса Едукатионксвдатапровидер</span><span class="sxs-lookup"><span data-stu-id="96663-103">educationCsvDataProvider resource type</span></span>

<span data-ttu-id="96663-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="96663-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96663-105">Используется для настройки профиля синхронизации данных School, когда CSV-файлы являются источником входных данных.</span><span class="sxs-lookup"><span data-stu-id="96663-105">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="96663-106">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="96663-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="96663-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="96663-107">Properties</span></span>

| <span data-ttu-id="96663-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="96663-108">Property</span></span> | <span data-ttu-id="96663-109">Тип</span><span class="sxs-lookup"><span data-stu-id="96663-109">Type</span></span> | <span data-ttu-id="96663-110">Описание</span><span class="sxs-lookup"><span data-stu-id="96663-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="96663-111">**настроек**</span><span class="sxs-lookup"><span data-stu-id="96663-111">**customizations**</span></span> | [<span data-ttu-id="96663-112">едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="96663-112">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="96663-113">Необязательные настройки, которые необходимо применить к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="96663-113">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96663-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96663-114">JSON representation</span></span>

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
