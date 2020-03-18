---
title: Тип ресурса Макоскернелекстенсион
description: Представляет конкретное расширение ядра macOS. Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef061b7a04b48b83df031abf6997900032307000
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42789215"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="0eea5-104">Тип ресурса Макоскернелекстенсион</span><span class="sxs-lookup"><span data-stu-id="0eea5-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="0eea5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eea5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eea5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0eea5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eea5-107">Представляет конкретное расширение ядра macOS.</span><span class="sxs-lookup"><span data-stu-id="0eea5-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="0eea5-108">Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.</span><span class="sxs-lookup"><span data-stu-id="0eea5-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="0eea5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0eea5-109">Properties</span></span>
|<span data-ttu-id="0eea5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0eea5-110">Property</span></span>|<span data-ttu-id="0eea5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0eea5-111">Type</span></span>|<span data-ttu-id="0eea5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0eea5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eea5-113">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="0eea5-113">teamIdentifier</span></span>|<span data-ttu-id="0eea5-114">String</span><span class="sxs-lookup"><span data-stu-id="0eea5-114">String</span></span>|<span data-ttu-id="0eea5-115">Идентификатор команды, использованный для подписи расширения ядра.</span><span class="sxs-lookup"><span data-stu-id="0eea5-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="0eea5-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="0eea5-116">bundleId</span></span>|<span data-ttu-id="0eea5-117">String</span><span class="sxs-lookup"><span data-stu-id="0eea5-117">String</span></span>|<span data-ttu-id="0eea5-118">Идентификатор пакета расширения ядра.</span><span class="sxs-lookup"><span data-stu-id="0eea5-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0eea5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="0eea5-119">Relationships</span></span>
<span data-ttu-id="0eea5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="0eea5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0eea5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0eea5-121">JSON Representation</span></span>
<span data-ttu-id="0eea5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0eea5-122">Here is a JSON representation of the resource.</span></span>
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



