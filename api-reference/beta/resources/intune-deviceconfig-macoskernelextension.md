---
title: Тип ресурса Макоскернелекстенсион
description: Представляет конкретное расширение ядра macOS. Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fbf12bd16bdf606010bc9b6518c8241fe28eb765
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321934"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="334c0-104">Тип ресурса Макоскернелекстенсион</span><span class="sxs-lookup"><span data-stu-id="334c0-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="334c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="334c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="334c0-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="334c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="334c0-107">Представляет конкретное расширение ядра macOS.</span><span class="sxs-lookup"><span data-stu-id="334c0-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="334c0-108">Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.</span><span class="sxs-lookup"><span data-stu-id="334c0-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="334c0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="334c0-109">Properties</span></span>
|<span data-ttu-id="334c0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="334c0-110">Property</span></span>|<span data-ttu-id="334c0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="334c0-111">Type</span></span>|<span data-ttu-id="334c0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="334c0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="334c0-113">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="334c0-113">teamIdentifier</span></span>|<span data-ttu-id="334c0-114">String</span><span class="sxs-lookup"><span data-stu-id="334c0-114">String</span></span>|<span data-ttu-id="334c0-115">Идентификатор команды, использованный для подписи расширения ядра.</span><span class="sxs-lookup"><span data-stu-id="334c0-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="334c0-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="334c0-116">bundleId</span></span>|<span data-ttu-id="334c0-117">String</span><span class="sxs-lookup"><span data-stu-id="334c0-117">String</span></span>|<span data-ttu-id="334c0-118">Идентификатор пакета расширения ядра.</span><span class="sxs-lookup"><span data-stu-id="334c0-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="334c0-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="334c0-119">Relationships</span></span>
<span data-ttu-id="334c0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="334c0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="334c0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="334c0-121">JSON Representation</span></span>
<span data-ttu-id="334c0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="334c0-122">Here is a JSON representation of the resource.</span></span>
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



