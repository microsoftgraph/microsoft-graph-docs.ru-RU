---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b3c115e312333a448318fb718140f5b6e8305494
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281833"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="97d67-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="97d67-103">macOSLobChildApp resource type</span></span>

<span data-ttu-id="97d67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97d67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97d67-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97d67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97d67-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97d67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d67-107">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="97d67-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="97d67-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="97d67-108">Properties</span></span>
|<span data-ttu-id="97d67-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="97d67-109">Property</span></span>|<span data-ttu-id="97d67-110">Тип</span><span class="sxs-lookup"><span data-stu-id="97d67-110">Type</span></span>|<span data-ttu-id="97d67-111">Описание</span><span class="sxs-lookup"><span data-stu-id="97d67-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d67-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="97d67-112">bundleId</span></span>|<span data-ttu-id="97d67-113">String</span><span class="sxs-lookup"><span data-stu-id="97d67-113">String</span></span>|<span data-ttu-id="97d67-114">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="97d67-114">The Identity Name.</span></span>|
|<span data-ttu-id="97d67-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="97d67-115">buildNumber</span></span>|<span data-ttu-id="97d67-116">String</span><span class="sxs-lookup"><span data-stu-id="97d67-116">String</span></span>|<span data-ttu-id="97d67-117">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="97d67-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="97d67-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="97d67-118">versionNumber</span></span>|<span data-ttu-id="97d67-119">String</span><span class="sxs-lookup"><span data-stu-id="97d67-119">String</span></span>|<span data-ttu-id="97d67-120">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="97d67-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97d67-121">Связи</span><span class="sxs-lookup"><span data-stu-id="97d67-121">Relationships</span></span>
<span data-ttu-id="97d67-122">Нет</span><span class="sxs-lookup"><span data-stu-id="97d67-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97d67-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97d67-123">JSON Representation</span></span>
<span data-ttu-id="97d67-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97d67-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




