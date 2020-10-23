---
title: Тип ресурса Манажеддевицесуммаризедаппстате
description: Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5171f99f557dd47f272bfb8c7c0629d9f907d974
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730327"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="c2e07-103">Тип ресурса Манажеддевицесуммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="c2e07-103">managedDeviceSummarizedAppState resource type</span></span>

<span data-ttu-id="c2e07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2e07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2e07-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2e07-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2e07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2e07-107">Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.</span><span class="sxs-lookup"><span data-stu-id="c2e07-107">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="c2e07-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2e07-108">Properties</span></span>
|<span data-ttu-id="c2e07-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2e07-109">Property</span></span>|<span data-ttu-id="c2e07-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2e07-110">Type</span></span>|<span data-ttu-id="c2e07-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2e07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2e07-112">суммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="c2e07-112">summarizedAppState</span></span>|[<span data-ttu-id="c2e07-113">рунстате</span><span class="sxs-lookup"><span data-stu-id="c2e07-113">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="c2e07-114">Рунстате для объекта.</span><span class="sxs-lookup"><span data-stu-id="c2e07-114">runState for the object.</span></span> <span data-ttu-id="c2e07-115">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="c2e07-115">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="c2e07-116">deviceId</span><span class="sxs-lookup"><span data-stu-id="c2e07-116">deviceId</span></span>|<span data-ttu-id="c2e07-117">String</span><span class="sxs-lookup"><span data-stu-id="c2e07-117">String</span></span>|<span data-ttu-id="c2e07-118">DeviceId устройства, представленного этим объектом</span><span class="sxs-lookup"><span data-stu-id="c2e07-118">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2e07-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c2e07-119">Relationships</span></span>
<span data-ttu-id="c2e07-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c2e07-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2e07-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2e07-121">JSON Representation</span></span>
<span data-ttu-id="c2e07-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2e07-122">Here is a JSON representation of the resource.</span></span>
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





