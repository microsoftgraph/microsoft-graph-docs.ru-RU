---
title: Тип ресурса Макоссистемекстенсионтипемаппинг
description: Представляет сопоставление между идентификаторами группы для расширений системы macOS и типов расширения системы.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3422cdac178ba22dee07aadb4700e2806eedc7ba
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179392"
---
# <a name="macossystemextensiontypemapping-resource-type"></a><span data-ttu-id="a559e-103">Тип ресурса Макоссистемекстенсионтипемаппинг</span><span class="sxs-lookup"><span data-stu-id="a559e-103">macOSSystemExtensionTypeMapping resource type</span></span>

<span data-ttu-id="a559e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a559e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a559e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a559e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a559e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a559e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a559e-107">Представляет сопоставление между идентификаторами группы для расширений системы macOS и типов расширения системы.</span><span class="sxs-lookup"><span data-stu-id="a559e-107">Represents a mapping between team identifiers for macOS system extensions and system extension types.</span></span>

## <a name="properties"></a><span data-ttu-id="a559e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a559e-108">Properties</span></span>
|<span data-ttu-id="a559e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a559e-109">Property</span></span>|<span data-ttu-id="a559e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a559e-110">Type</span></span>|<span data-ttu-id="a559e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a559e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a559e-112">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="a559e-112">teamIdentifier</span></span>|<span data-ttu-id="a559e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a559e-113">String</span></span>|<span data-ttu-id="a559e-114">Получает или задает идентификатор группы, используемый для подписи расширения системы.</span><span class="sxs-lookup"><span data-stu-id="a559e-114">Gets or sets the team identifier used to sign the system extension.</span></span>|
|<span data-ttu-id="a559e-115">алловедтипес</span><span class="sxs-lookup"><span data-stu-id="a559e-115">allowedTypes</span></span>|[<span data-ttu-id="a559e-116">макоссистемекстенсионтипе</span><span class="sxs-lookup"><span data-stu-id="a559e-116">macOSSystemExtensionType</span></span>](../resources/intune-deviceconfig-macossystemextensiontype.md)|<span data-ttu-id="a559e-117">Получает или задает разрешенные типы расширений системы macOS.</span><span class="sxs-lookup"><span data-stu-id="a559e-117">Gets or sets the allowed macOS system extension types.</span></span> <span data-ttu-id="a559e-118">Возможные значения: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span><span class="sxs-lookup"><span data-stu-id="a559e-118">Possible values are: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a559e-119">Связи</span><span class="sxs-lookup"><span data-stu-id="a559e-119">Relationships</span></span>
<span data-ttu-id="a559e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a559e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a559e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a559e-121">JSON Representation</span></span>
<span data-ttu-id="a559e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a559e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtensionTypeMapping",
  "teamIdentifier": "String",
  "allowedTypes": "String"
}
```



