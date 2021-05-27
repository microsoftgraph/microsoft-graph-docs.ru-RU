---
title: тип ресурса ticketInfo
description: Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a59b62ddb014dedd802af6fcde001d4791d729c3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682602"
---
# <a name="ticketinfo-resource-type"></a><span data-ttu-id="15e53-103">тип ресурса ticketInfo</span><span class="sxs-lookup"><span data-stu-id="15e53-103">ticketInfo resource type</span></span>

<span data-ttu-id="15e53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15e53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15e53-105">Объект, который представляет сведения о билетах, связанные с запросами на назначение ролей</span><span class="sxs-lookup"><span data-stu-id="15e53-105">The object that represents ticket information related to role assignment requests</span></span>

## <a name="properties"></a><span data-ttu-id="15e53-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="15e53-106">Properties</span></span>
|<span data-ttu-id="15e53-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="15e53-107">Property</span></span>|<span data-ttu-id="15e53-108">Тип</span><span class="sxs-lookup"><span data-stu-id="15e53-108">Type</span></span>|<span data-ttu-id="15e53-109">Описание</span><span class="sxs-lookup"><span data-stu-id="15e53-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15e53-110">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="15e53-110">ticketNumber</span></span>|<span data-ttu-id="15e53-111">String</span><span class="sxs-lookup"><span data-stu-id="15e53-111">String</span></span>|<span data-ttu-id="15e53-112">Метаданные номеров билетов</span><span class="sxs-lookup"><span data-stu-id="15e53-112">Ticket number meta data</span></span>|
|<span data-ttu-id="15e53-113">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="15e53-113">ticketSystem</span></span>|<span data-ttu-id="15e53-114">String</span><span class="sxs-lookup"><span data-stu-id="15e53-114">String</span></span>|<span data-ttu-id="15e53-115">Метаданные системы билетов</span><span class="sxs-lookup"><span data-stu-id="15e53-115">Ticket system meta data</span></span>|

## <a name="relationships"></a><span data-ttu-id="15e53-116">Связи</span><span class="sxs-lookup"><span data-stu-id="15e53-116">Relationships</span></span>
<span data-ttu-id="15e53-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="15e53-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15e53-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="15e53-118">JSON representation</span></span>
<span data-ttu-id="15e53-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15e53-119">The following is a JSON representation of the resource.</span></span>
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

