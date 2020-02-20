---
title: Тип ресурса Манажеддевицесуммаризедаппстате
description: Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76020e9028207d15cf198d9c4401abc4819a1ffd
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161295"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="a3eb0-103">Тип ресурса Манажеддевицесуммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="a3eb0-103">managedDeviceSummarizedAppState resource type</span></span>

> <span data-ttu-id="a3eb0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3eb0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3eb0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3eb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3eb0-106">Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.</span><span class="sxs-lookup"><span data-stu-id="a3eb0-106">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="a3eb0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3eb0-107">Properties</span></span>
|<span data-ttu-id="a3eb0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3eb0-108">Property</span></span>|<span data-ttu-id="a3eb0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a3eb0-109">Type</span></span>|<span data-ttu-id="a3eb0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3eb0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3eb0-111">суммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="a3eb0-111">summarizedAppState</span></span>|[<span data-ttu-id="a3eb0-112">рунстате</span><span class="sxs-lookup"><span data-stu-id="a3eb0-112">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="a3eb0-113">Рунстате для объекта.</span><span class="sxs-lookup"><span data-stu-id="a3eb0-113">runState for the object.</span></span> <span data-ttu-id="a3eb0-114">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="a3eb0-114">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="a3eb0-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="a3eb0-115">deviceId</span></span>|<span data-ttu-id="a3eb0-116">String</span><span class="sxs-lookup"><span data-stu-id="a3eb0-116">String</span></span>|<span data-ttu-id="a3eb0-117">DeviceId устройства, представленного этим объектом</span><span class="sxs-lookup"><span data-stu-id="a3eb0-117">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3eb0-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="a3eb0-118">Relationships</span></span>
<span data-ttu-id="a3eb0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a3eb0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3eb0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3eb0-120">JSON Representation</span></span>
<span data-ttu-id="a3eb0-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3eb0-121">Here is a JSON representation of the resource.</span></span>
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



