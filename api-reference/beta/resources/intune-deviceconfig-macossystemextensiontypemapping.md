---
title: Тип ресурса Макоссистемекстенсионтипемаппинг
description: Представляет сопоставление между идентификаторами группы для расширений системы macOS и типов расширения системы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f827ecd186268991d499f30b8ff39f43c3d8103
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064152"
---
# <a name="macossystemextensiontypemapping-resource-type"></a><span data-ttu-id="058d2-103">Тип ресурса Макоссистемекстенсионтипемаппинг</span><span class="sxs-lookup"><span data-stu-id="058d2-103">macOSSystemExtensionTypeMapping resource type</span></span>

<span data-ttu-id="058d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="058d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="058d2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="058d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="058d2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="058d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="058d2-107">Представляет сопоставление между идентификаторами группы для расширений системы macOS и типов расширения системы.</span><span class="sxs-lookup"><span data-stu-id="058d2-107">Represents a mapping between team identifiers for macOS system extensions and system extension types.</span></span>

## <a name="properties"></a><span data-ttu-id="058d2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="058d2-108">Properties</span></span>
|<span data-ttu-id="058d2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="058d2-109">Property</span></span>|<span data-ttu-id="058d2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="058d2-110">Type</span></span>|<span data-ttu-id="058d2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="058d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="058d2-112">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="058d2-112">teamIdentifier</span></span>|<span data-ttu-id="058d2-113">String</span><span class="sxs-lookup"><span data-stu-id="058d2-113">String</span></span>|<span data-ttu-id="058d2-114">Получает или задает идентификатор группы, используемый для подписи расширения системы.</span><span class="sxs-lookup"><span data-stu-id="058d2-114">Gets or sets the team identifier used to sign the system extension.</span></span>|
|<span data-ttu-id="058d2-115">алловедтипес</span><span class="sxs-lookup"><span data-stu-id="058d2-115">allowedTypes</span></span>|[<span data-ttu-id="058d2-116">macOSSystemExtensionType</span><span class="sxs-lookup"><span data-stu-id="058d2-116">macOSSystemExtensionType</span></span>](../resources/intune-deviceconfig-macossystemextensiontype.md)|<span data-ttu-id="058d2-117">Получает или задает разрешенные типы расширений системы macOS.</span><span class="sxs-lookup"><span data-stu-id="058d2-117">Gets or sets the allowed macOS system extension types.</span></span> <span data-ttu-id="058d2-118">Возможные значения: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span><span class="sxs-lookup"><span data-stu-id="058d2-118">Possible values are: `driverExtensionsAllowed`, `networkExtensionsAllowed`, `endpointSecurityExtensionsAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="058d2-119">Связи</span><span class="sxs-lookup"><span data-stu-id="058d2-119">Relationships</span></span>
<span data-ttu-id="058d2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="058d2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="058d2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="058d2-121">JSON Representation</span></span>
<span data-ttu-id="058d2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="058d2-122">Here is a JSON representation of the resource.</span></span>
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






