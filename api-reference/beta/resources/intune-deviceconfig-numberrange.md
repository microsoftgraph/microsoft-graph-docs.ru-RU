---
title: Тип ресурса Нумберранже
description: Определение диапазона номеров.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e47252b42fe7be886a1d6ce7c0d71b6c2dc1b21
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460963"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="1d9ae-103">Тип ресурса Нумберранже</span><span class="sxs-lookup"><span data-stu-id="1d9ae-103">numberRange resource type</span></span>

<span data-ttu-id="1d9ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d9ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d9ae-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d9ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d9ae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d9ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d9ae-107">Определение диапазона номеров.</span><span class="sxs-lookup"><span data-stu-id="1d9ae-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1d9ae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d9ae-108">Properties</span></span>
|<span data-ttu-id="1d9ae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d9ae-109">Property</span></span>|<span data-ttu-id="1d9ae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1d9ae-110">Type</span></span>|<span data-ttu-id="1d9ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1d9ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d9ae-112">ловернумбер</span><span class="sxs-lookup"><span data-stu-id="1d9ae-112">lowerNumber</span></span>|<span data-ttu-id="1d9ae-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1d9ae-113">Int32</span></span>|<span data-ttu-id="1d9ae-114">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="1d9ae-114">Lower number.</span></span>|
|<span data-ttu-id="1d9ae-115">уппернумбер</span><span class="sxs-lookup"><span data-stu-id="1d9ae-115">upperNumber</span></span>|<span data-ttu-id="1d9ae-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1d9ae-116">Int32</span></span>|<span data-ttu-id="1d9ae-117">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="1d9ae-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d9ae-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1d9ae-118">Relationships</span></span>
<span data-ttu-id="1d9ae-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1d9ae-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d9ae-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d9ae-120">JSON Representation</span></span>
<span data-ttu-id="1d9ae-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d9ae-121">Here is a JSON representation of the resource.</span></span>
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



