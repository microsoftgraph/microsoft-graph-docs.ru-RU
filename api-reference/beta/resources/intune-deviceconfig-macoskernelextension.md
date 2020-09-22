---
title: Тип ресурса Макоскернелекстенсион
description: Представляет конкретное расширение ядра macOS. Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ef7004fd7be5340a7e5a1614e51d3ecdfd6f7ff4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024110"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="9fed8-104">Тип ресурса Макоскернелекстенсион</span><span class="sxs-lookup"><span data-stu-id="9fed8-104">macOSKernelExtension resource type</span></span>

<span data-ttu-id="9fed8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fed8-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fed8-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fed8-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fed8-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fed8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fed8-108">Представляет конкретное расширение ядра macOS.</span><span class="sxs-lookup"><span data-stu-id="9fed8-108">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="9fed8-109">Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.</span><span class="sxs-lookup"><span data-stu-id="9fed8-109">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="9fed8-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fed8-110">Properties</span></span>
|<span data-ttu-id="9fed8-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fed8-111">Property</span></span>|<span data-ttu-id="9fed8-112">Тип</span><span class="sxs-lookup"><span data-stu-id="9fed8-112">Type</span></span>|<span data-ttu-id="9fed8-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9fed8-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fed8-114">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="9fed8-114">teamIdentifier</span></span>|<span data-ttu-id="9fed8-115">String</span><span class="sxs-lookup"><span data-stu-id="9fed8-115">String</span></span>|<span data-ttu-id="9fed8-116">Идентификатор команды, использованный для подписи расширения ядра.</span><span class="sxs-lookup"><span data-stu-id="9fed8-116">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="9fed8-117">bundleId</span><span class="sxs-lookup"><span data-stu-id="9fed8-117">bundleId</span></span>|<span data-ttu-id="9fed8-118">String</span><span class="sxs-lookup"><span data-stu-id="9fed8-118">String</span></span>|<span data-ttu-id="9fed8-119">Идентификатор пакета расширения ядра.</span><span class="sxs-lookup"><span data-stu-id="9fed8-119">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fed8-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="9fed8-120">Relationships</span></span>
<span data-ttu-id="9fed8-121">Нет</span><span class="sxs-lookup"><span data-stu-id="9fed8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fed8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fed8-122">JSON Representation</span></span>
<span data-ttu-id="9fed8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fed8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```






