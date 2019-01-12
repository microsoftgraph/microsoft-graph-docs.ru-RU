---
title: Тип ресурса educationCsvDataProvider
description: 'Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ef77671f862a0b59b5697b76bb54dc20e42856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952757"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="5da3c-103">Тип ресурса educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="5da3c-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="5da3c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5da3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5da3c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5da3c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5da3c-106">Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.</span><span class="sxs-lookup"><span data-stu-id="5da3c-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="5da3c-107">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="5da3c-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5da3c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5da3c-108">Properties</span></span>

| <span data-ttu-id="5da3c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5da3c-109">Property</span></span> | <span data-ttu-id="5da3c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5da3c-110">Type</span></span> | <span data-ttu-id="5da3c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5da3c-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5da3c-112">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="5da3c-112">**customizations**</span></span> | [<span data-ttu-id="5da3c-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="5da3c-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="5da3c-114">Необязательный настроек применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="5da3c-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5da3c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5da3c-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
