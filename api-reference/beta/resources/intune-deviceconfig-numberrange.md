---
title: Тип ресурса numberRange
description: Определение номер диапазона.
ms.openlocfilehash: ef4b24e3034414221365d81c40b453e7ca66a94b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075148"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="45657-103">Тип ресурса numberRange</span><span class="sxs-lookup"><span data-stu-id="45657-103">numberRange resource type</span></span>

> <span data-ttu-id="45657-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45657-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45657-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45657-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45657-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45657-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45657-107">Определение номер диапазона.</span><span class="sxs-lookup"><span data-stu-id="45657-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="45657-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="45657-108">Properties</span></span>
|<span data-ttu-id="45657-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="45657-109">Property</span></span>|<span data-ttu-id="45657-110">Тип</span><span class="sxs-lookup"><span data-stu-id="45657-110">Type</span></span>|<span data-ttu-id="45657-111">Description</span><span class="sxs-lookup"><span data-stu-id="45657-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45657-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="45657-112">lowerNumber</span></span>|<span data-ttu-id="45657-113">Int32</span><span class="sxs-lookup"><span data-stu-id="45657-113">Int32</span></span>|<span data-ttu-id="45657-114">Меньшее число.</span><span class="sxs-lookup"><span data-stu-id="45657-114">Lower number.</span></span>|
|<span data-ttu-id="45657-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="45657-115">upperNumber</span></span>|<span data-ttu-id="45657-116">Int32</span><span class="sxs-lookup"><span data-stu-id="45657-116">Int32</span></span>|<span data-ttu-id="45657-117">Верхний номер.</span><span class="sxs-lookup"><span data-stu-id="45657-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45657-118">Связи</span><span class="sxs-lookup"><span data-stu-id="45657-118">Relationships</span></span>
<span data-ttu-id="45657-119">Нет</span><span class="sxs-lookup"><span data-stu-id="45657-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="45657-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45657-120">JSON Representation</span></span>
<span data-ttu-id="45657-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45657-121">Here is a JSON representation of the resource.</span></span>
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





