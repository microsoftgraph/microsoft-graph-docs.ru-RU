---
title: Тип ресурса educationCsvDataProvider
description: 'Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.  '
author: mmast-msft
ms.openlocfilehash: 1a816d4e176147d549381465154e35cf0a821b98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317901"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="8678d-103">Тип ресурса educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="8678d-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="8678d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8678d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8678d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8678d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8678d-106">Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.</span><span class="sxs-lookup"><span data-stu-id="8678d-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="8678d-107">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="8678d-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8678d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8678d-108">Properties</span></span>

| <span data-ttu-id="8678d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8678d-109">Property</span></span> | <span data-ttu-id="8678d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8678d-110">Type</span></span> | <span data-ttu-id="8678d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8678d-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8678d-112">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="8678d-112">**customizations**</span></span> | [<span data-ttu-id="8678d-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="8678d-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="8678d-114">Необязательный настроек применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="8678d-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8678d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8678d-115">JSON representation</span></span>

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
