---
title: Тип ресурса assignmentFilterValidationResult
description: Представляет результат проверки API.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a540bdec4265c544f565e560b6858755d0076178
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160956"
---
# <a name="assignmentfiltervalidationresult-resource-type"></a><span data-ttu-id="03697-103">Тип ресурса assignmentFilterValidationResult</span><span class="sxs-lookup"><span data-stu-id="03697-103">assignmentFilterValidationResult resource type</span></span>

<span data-ttu-id="03697-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03697-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03697-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03697-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03697-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03697-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03697-107">Представляет результат проверки API.</span><span class="sxs-lookup"><span data-stu-id="03697-107">Represents result of Validation API.</span></span>

## <a name="properties"></a><span data-ttu-id="03697-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="03697-108">Properties</span></span>
|<span data-ttu-id="03697-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="03697-109">Property</span></span>|<span data-ttu-id="03697-110">Тип</span><span class="sxs-lookup"><span data-stu-id="03697-110">Type</span></span>|<span data-ttu-id="03697-111">Описание</span><span class="sxs-lookup"><span data-stu-id="03697-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03697-112">isValidRule</span><span class="sxs-lookup"><span data-stu-id="03697-112">isValidRule</span></span>|<span data-ttu-id="03697-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="03697-113">Boolean</span></span>|<span data-ttu-id="03697-114">Индикатор допустимым или недопустимым правилом.</span><span class="sxs-lookup"><span data-stu-id="03697-114">Indicator to valid or invalid rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03697-115">Связи</span><span class="sxs-lookup"><span data-stu-id="03697-115">Relationships</span></span>
<span data-ttu-id="03697-116">Нет</span><span class="sxs-lookup"><span data-stu-id="03697-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03697-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03697-117">JSON Representation</span></span>
<span data-ttu-id="03697-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03697-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterValidationResult",
  "isValidRule": true
}
```




