---
title: Тип ресурса Манажеддевицесуммаризедаппстате
description: Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e6439ad781ad83bcae5bd66bc83f7a566e3b2ea6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765155"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="aaf96-103">Тип ресурса Манажеддевицесуммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="aaf96-103">managedDeviceSummarizedAppState resource type</span></span>

> <span data-ttu-id="aaf96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaf96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaf96-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aaf96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaf96-106">Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.</span><span class="sxs-lookup"><span data-stu-id="aaf96-106">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="aaf96-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aaf96-107">Properties</span></span>
|<span data-ttu-id="aaf96-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aaf96-108">Property</span></span>|<span data-ttu-id="aaf96-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aaf96-109">Type</span></span>|<span data-ttu-id="aaf96-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aaf96-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaf96-111">суммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="aaf96-111">summarizedAppState</span></span>|[<span data-ttu-id="aaf96-112">рунстате</span><span class="sxs-lookup"><span data-stu-id="aaf96-112">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="aaf96-113">Рунстате для объекта.</span><span class="sxs-lookup"><span data-stu-id="aaf96-113">runState for the object.</span></span> <span data-ttu-id="aaf96-114">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="aaf96-114">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="aaf96-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="aaf96-115">deviceId</span></span>|<span data-ttu-id="aaf96-116">String</span><span class="sxs-lookup"><span data-stu-id="aaf96-116">String</span></span>|<span data-ttu-id="aaf96-117">DeviceId устройства, представленного этим объектом</span><span class="sxs-lookup"><span data-stu-id="aaf96-117">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaf96-118">Связи</span><span class="sxs-lookup"><span data-stu-id="aaf96-118">Relationships</span></span>
<span data-ttu-id="aaf96-119">Нет</span><span class="sxs-lookup"><span data-stu-id="aaf96-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aaf96-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aaf96-120">JSON Representation</span></span>
<span data-ttu-id="aaf96-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aaf96-121">Here is a JSON representation of the resource.</span></span>
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



