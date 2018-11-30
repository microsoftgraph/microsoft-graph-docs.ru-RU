---
title: Тип ресурса keyValue
description: Определение значения ключа.
ms.openlocfilehash: 7279b48243139b9234b737ceb7d7fb1ad7232451
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077241"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="0f2e0-103">Тип ресурса keyValue</span><span class="sxs-lookup"><span data-stu-id="0f2e0-103">keyValue resource type</span></span>

> <span data-ttu-id="0f2e0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f2e0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f2e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f2e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f2e0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f2e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f2e0-107">Определение значения ключа.</span><span class="sxs-lookup"><span data-stu-id="0f2e0-107">Key Value definition.</span></span>
## <a name="properties"></a><span data-ttu-id="0f2e0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f2e0-108">Properties</span></span>
|<span data-ttu-id="0f2e0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f2e0-109">Property</span></span>|<span data-ttu-id="0f2e0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f2e0-110">Type</span></span>|<span data-ttu-id="0f2e0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f2e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f2e0-112">key</span><span class="sxs-lookup"><span data-stu-id="0f2e0-112">key</span></span>|<span data-ttu-id="0f2e0-113">String</span><span class="sxs-lookup"><span data-stu-id="0f2e0-113">String</span></span>|<span data-ttu-id="0f2e0-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="0f2e0-114">Key.</span></span>|
|<span data-ttu-id="0f2e0-115">value</span><span class="sxs-lookup"><span data-stu-id="0f2e0-115">value</span></span>|<span data-ttu-id="0f2e0-116">String</span><span class="sxs-lookup"><span data-stu-id="0f2e0-116">String</span></span>|<span data-ttu-id="0f2e0-117">Значение</span><span class="sxs-lookup"><span data-stu-id="0f2e0-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f2e0-118">Связи</span><span class="sxs-lookup"><span data-stu-id="0f2e0-118">Relationships</span></span>
<span data-ttu-id="0f2e0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0f2e0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f2e0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f2e0-120">JSON Representation</span></span>
<span data-ttu-id="0f2e0-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f2e0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```





