---
title: Тип ресурса Макоскернелекстенсион
description: Представляет конкретное расширение ядра macOS. Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04320f92045ae128ca1bf128484d2aa55f03d706
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570647"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="f09cd-104">Тип ресурса Макоскернелекстенсион</span><span class="sxs-lookup"><span data-stu-id="f09cd-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="f09cd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f09cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f09cd-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f09cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f09cd-107">Представляет конкретное расширение ядра macOS.</span><span class="sxs-lookup"><span data-stu-id="f09cd-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="f09cd-108">Расширение ядра macOS можно описать с помощью идентификатора группы и идентификатора пакета.</span><span class="sxs-lookup"><span data-stu-id="f09cd-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="f09cd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f09cd-109">Properties</span></span>
|<span data-ttu-id="f09cd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f09cd-110">Property</span></span>|<span data-ttu-id="f09cd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f09cd-111">Type</span></span>|<span data-ttu-id="f09cd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f09cd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f09cd-113">Теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="f09cd-113">teamIdentifier</span></span>|<span data-ttu-id="f09cd-114">String</span><span class="sxs-lookup"><span data-stu-id="f09cd-114">String</span></span>|<span data-ttu-id="f09cd-115">Идентификатор команды, использованный для подписи расширения ядра.</span><span class="sxs-lookup"><span data-stu-id="f09cd-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="f09cd-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="f09cd-116">bundleId</span></span>|<span data-ttu-id="f09cd-117">String</span><span class="sxs-lookup"><span data-stu-id="f09cd-117">String</span></span>|<span data-ttu-id="f09cd-118">Идентификатор пакета расширения ядра.</span><span class="sxs-lookup"><span data-stu-id="f09cd-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f09cd-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="f09cd-119">Relationships</span></span>
<span data-ttu-id="f09cd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f09cd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f09cd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f09cd-121">JSON Representation</span></span>
<span data-ttu-id="f09cd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f09cd-122">Here is a JSON representation of the resource.</span></span>
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





