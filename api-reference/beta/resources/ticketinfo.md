---
title: тип ресурса ticketInfo
description: Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 584600bf017a75efb141539b6f1397920717fb76
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299761"
---
# <a name="ticketinfo-resource-type"></a><span data-ttu-id="7bc1e-103">тип ресурса ticketInfo</span><span class="sxs-lookup"><span data-stu-id="7bc1e-103">ticketInfo resource type</span></span>

<span data-ttu-id="7bc1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bc1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bc1e-105">Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей</span><span class="sxs-lookup"><span data-stu-id="7bc1e-105">The object that represents ticket information related to role assignment requests</span></span>

## <a name="properties"></a><span data-ttu-id="7bc1e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bc1e-106">Properties</span></span>
|<span data-ttu-id="7bc1e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bc1e-107">Property</span></span>|<span data-ttu-id="7bc1e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7bc1e-108">Type</span></span>|<span data-ttu-id="7bc1e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7bc1e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bc1e-110">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="7bc1e-110">ticketNumber</span></span>|<span data-ttu-id="7bc1e-111">Строка</span><span class="sxs-lookup"><span data-stu-id="7bc1e-111">String</span></span>|<span data-ttu-id="7bc1e-112">Метаданные номеров билетов</span><span class="sxs-lookup"><span data-stu-id="7bc1e-112">Ticket number meta data</span></span>|
|<span data-ttu-id="7bc1e-113">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="7bc1e-113">ticketSystem</span></span>|<span data-ttu-id="7bc1e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="7bc1e-114">String</span></span>|<span data-ttu-id="7bc1e-115">Метаданные системы билетов</span><span class="sxs-lookup"><span data-stu-id="7bc1e-115">Ticket system meta data</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bc1e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="7bc1e-116">Relationships</span></span>
<span data-ttu-id="7bc1e-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7bc1e-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bc1e-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7bc1e-118">JSON representation</span></span>
<span data-ttu-id="7bc1e-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bc1e-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ticketInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ticketInfo",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

