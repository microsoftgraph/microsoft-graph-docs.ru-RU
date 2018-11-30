---
title: Тип ресурса educationCsvDataProvider
description: 'Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.  '
ms.openlocfilehash: a3079b4f18c74c95fb0f8646116f2c7901d17b3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075198"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="b090b-103">Тип ресурса educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="b090b-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="b090b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b090b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b090b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b090b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b090b-106">Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.</span><span class="sxs-lookup"><span data-stu-id="b090b-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="b090b-107">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b090b-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b090b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b090b-108">Properties</span></span>

| <span data-ttu-id="b090b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b090b-109">Property</span></span> | <span data-ttu-id="b090b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b090b-110">Type</span></span> | <span data-ttu-id="b090b-111">Description</span><span class="sxs-lookup"><span data-stu-id="b090b-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b090b-112">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="b090b-112">**customizations**</span></span> | [<span data-ttu-id="b090b-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="b090b-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="b090b-114">Необязательный настроек применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="b090b-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b090b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b090b-115">JSON representation</span></span>

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
