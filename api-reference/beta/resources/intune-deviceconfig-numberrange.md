---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 225dc4a48e0f95ccf1fdeae828c1ec603ed68802
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542279"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="fc4d6-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="fc4d6-103">numberRange resource type</span></span>

> <span data-ttu-id="fc4d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc4d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc4d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc4d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc4d6-106">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="fc4d6-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="fc4d6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc4d6-107">Properties</span></span>
|<span data-ttu-id="fc4d6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc4d6-108">Property</span></span>|<span data-ttu-id="fc4d6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fc4d6-109">Type</span></span>|<span data-ttu-id="fc4d6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc4d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc4d6-111">Ловернумбер</span><span class="sxs-lookup"><span data-stu-id="fc4d6-111">lowerNumber</span></span>|<span data-ttu-id="fc4d6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fc4d6-112">Int32</span></span>|<span data-ttu-id="fc4d6-113">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="fc4d6-113">Lower number.</span></span>|
|<span data-ttu-id="fc4d6-114">Уппернумбер</span><span class="sxs-lookup"><span data-stu-id="fc4d6-114">upperNumber</span></span>|<span data-ttu-id="fc4d6-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fc4d6-115">Int32</span></span>|<span data-ttu-id="fc4d6-116">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="fc4d6-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc4d6-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="fc4d6-117">Relationships</span></span>
<span data-ttu-id="fc4d6-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fc4d6-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc4d6-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc4d6-119">JSON Representation</span></span>
<span data-ttu-id="fc4d6-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc4d6-120">Here is a JSON representation of the resource.</span></span>
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





