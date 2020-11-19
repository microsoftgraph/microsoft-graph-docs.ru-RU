---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c9c3b4f286bb9c3fa68beb24dd395e28d9633d4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273237"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="ba262-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="ba262-103">numberRange resource type</span></span>

<span data-ttu-id="ba262-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba262-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba262-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba262-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba262-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba262-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba262-107">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="ba262-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="ba262-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba262-108">Properties</span></span>
|<span data-ttu-id="ba262-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba262-109">Property</span></span>|<span data-ttu-id="ba262-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ba262-110">Type</span></span>|<span data-ttu-id="ba262-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ba262-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba262-112">ловернумбер</span><span class="sxs-lookup"><span data-stu-id="ba262-112">lowerNumber</span></span>|<span data-ttu-id="ba262-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ba262-113">Int32</span></span>|<span data-ttu-id="ba262-114">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="ba262-114">Lower number.</span></span>|
|<span data-ttu-id="ba262-115">уппернумбер</span><span class="sxs-lookup"><span data-stu-id="ba262-115">upperNumber</span></span>|<span data-ttu-id="ba262-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ba262-116">Int32</span></span>|<span data-ttu-id="ba262-117">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="ba262-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba262-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ba262-118">Relationships</span></span>
<span data-ttu-id="ba262-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ba262-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba262-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba262-120">JSON Representation</span></span>
<span data-ttu-id="ba262-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba262-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```




