---
title: Тип ресурса Манажеддевицесуммаризедаппстате
description: Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: db00f874f6a2db1c4792955a3cbc2e5f32a81a0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523361"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="26f58-103">Тип ресурса Манажеддевицесуммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="26f58-103">managedDeviceSummarizedAppState resource type</span></span>

<span data-ttu-id="26f58-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="26f58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26f58-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26f58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26f58-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26f58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26f58-107">Событие, представляющее устройства пользователя с невыполненными или ожидающими приложениями.</span><span class="sxs-lookup"><span data-stu-id="26f58-107">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="26f58-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="26f58-108">Properties</span></span>
|<span data-ttu-id="26f58-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="26f58-109">Property</span></span>|<span data-ttu-id="26f58-110">Тип</span><span class="sxs-lookup"><span data-stu-id="26f58-110">Type</span></span>|<span data-ttu-id="26f58-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26f58-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26f58-112">суммаризедаппстате</span><span class="sxs-lookup"><span data-stu-id="26f58-112">summarizedAppState</span></span>|[<span data-ttu-id="26f58-113">рунстате</span><span class="sxs-lookup"><span data-stu-id="26f58-113">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="26f58-114">Рунстате для объекта.</span><span class="sxs-lookup"><span data-stu-id="26f58-114">runState for the object.</span></span> <span data-ttu-id="26f58-115">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="26f58-115">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="26f58-116">deviceId</span><span class="sxs-lookup"><span data-stu-id="26f58-116">deviceId</span></span>|<span data-ttu-id="26f58-117">String</span><span class="sxs-lookup"><span data-stu-id="26f58-117">String</span></span>|<span data-ttu-id="26f58-118">DeviceId устройства, представленного этим объектом</span><span class="sxs-lookup"><span data-stu-id="26f58-118">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="26f58-119">Связи</span><span class="sxs-lookup"><span data-stu-id="26f58-119">Relationships</span></span>
<span data-ttu-id="26f58-120">Нет</span><span class="sxs-lookup"><span data-stu-id="26f58-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26f58-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26f58-121">JSON Representation</span></span>
<span data-ttu-id="26f58-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26f58-122">Here is a JSON representation of the resource.</span></span>
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



