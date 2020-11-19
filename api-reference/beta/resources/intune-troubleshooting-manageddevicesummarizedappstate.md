---
title: Тип ресурса Манажеддевицесуммаризедаппстате
description: Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4727477497657a917906f9b778fa76647fc394d9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271606"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="93277-103">Тип ресурса Манажеддевицесуммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="93277-103">managedDeviceSummarizedAppState resource type</span></span>

<span data-ttu-id="93277-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93277-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93277-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93277-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93277-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93277-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93277-107">Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.</span><span class="sxs-lookup"><span data-stu-id="93277-107">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="93277-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="93277-108">Properties</span></span>
|<span data-ttu-id="93277-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="93277-109">Property</span></span>|<span data-ttu-id="93277-110">Тип</span><span class="sxs-lookup"><span data-stu-id="93277-110">Type</span></span>|<span data-ttu-id="93277-111">Описание</span><span class="sxs-lookup"><span data-stu-id="93277-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93277-112">суммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="93277-112">summarizedAppState</span></span>|[<span data-ttu-id="93277-113">рунстате</span><span class="sxs-lookup"><span data-stu-id="93277-113">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="93277-114">Рунстате для объекта.</span><span class="sxs-lookup"><span data-stu-id="93277-114">runState for the object.</span></span> <span data-ttu-id="93277-115">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="93277-115">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="93277-116">deviceId</span><span class="sxs-lookup"><span data-stu-id="93277-116">deviceId</span></span>|<span data-ttu-id="93277-117">String</span><span class="sxs-lookup"><span data-stu-id="93277-117">String</span></span>|<span data-ttu-id="93277-118">DeviceId устройства, представленного этим объектом</span><span class="sxs-lookup"><span data-stu-id="93277-118">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="93277-119">Связи</span><span class="sxs-lookup"><span data-stu-id="93277-119">Relationships</span></span>
<span data-ttu-id="93277-120">Нет</span><span class="sxs-lookup"><span data-stu-id="93277-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93277-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93277-121">JSON Representation</span></span>
<span data-ttu-id="93277-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93277-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceSummarizedAppState",
  "summarizedAppState": "String",
  "deviceId": "String"
}
```




