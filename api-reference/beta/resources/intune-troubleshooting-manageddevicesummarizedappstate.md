---
title: Тип ресурса Манажеддевицесуммаризедаппстате
description: Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 957d25e9b5dfe333529f228eecddb937b1752c2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385717"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="74765-103">Тип ресурса Манажеддевицесуммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="74765-103">managedDeviceSummarizedAppState resource type</span></span>

<span data-ttu-id="74765-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74765-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74765-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74765-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74765-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74765-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74765-107">Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.</span><span class="sxs-lookup"><span data-stu-id="74765-107">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="74765-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="74765-108">Properties</span></span>
|<span data-ttu-id="74765-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="74765-109">Property</span></span>|<span data-ttu-id="74765-110">Тип</span><span class="sxs-lookup"><span data-stu-id="74765-110">Type</span></span>|<span data-ttu-id="74765-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74765-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74765-112">суммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="74765-112">summarizedAppState</span></span>|[<span data-ttu-id="74765-113">рунстате</span><span class="sxs-lookup"><span data-stu-id="74765-113">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="74765-114">Рунстате для объекта.</span><span class="sxs-lookup"><span data-stu-id="74765-114">runState for the object.</span></span> <span data-ttu-id="74765-115">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="74765-115">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="74765-116">deviceId</span><span class="sxs-lookup"><span data-stu-id="74765-116">deviceId</span></span>|<span data-ttu-id="74765-117">String</span><span class="sxs-lookup"><span data-stu-id="74765-117">String</span></span>|<span data-ttu-id="74765-118">DeviceId устройства, представленного этим объектом</span><span class="sxs-lookup"><span data-stu-id="74765-118">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="74765-119">Связи</span><span class="sxs-lookup"><span data-stu-id="74765-119">Relationships</span></span>
<span data-ttu-id="74765-120">Нет</span><span class="sxs-lookup"><span data-stu-id="74765-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74765-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74765-121">JSON Representation</span></span>
<span data-ttu-id="74765-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74765-122">Here is a JSON representation of the resource.</span></span>
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



