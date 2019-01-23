---
title: Тип ресурса educationCsvDataProvider
description: 'Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c9211d5f7ca25b78c6e76c3744f6941e3b172bb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399348"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="4faeb-103">Тип ресурса educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="4faeb-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="4faeb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4faeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4faeb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4faeb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4faeb-106">Используется для настройки синхронизации профилей данных school после ввода источника файлов CSV.</span><span class="sxs-lookup"><span data-stu-id="4faeb-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="4faeb-107">На основе [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="4faeb-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4faeb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4faeb-108">Properties</span></span>

| <span data-ttu-id="4faeb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4faeb-109">Property</span></span> | <span data-ttu-id="4faeb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4faeb-110">Type</span></span> | <span data-ttu-id="4faeb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4faeb-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4faeb-112">**пользовательских настроек**</span><span class="sxs-lookup"><span data-stu-id="4faeb-112">**customizations**</span></span> | [<span data-ttu-id="4faeb-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="4faeb-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="4faeb-114">Необязательный настроек применяется для синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="4faeb-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4faeb-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4faeb-115">JSON representation</span></span>

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
