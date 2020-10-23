---
title: Тип ресурса Макослобчилдапп
description: Содержит свойства бизнес-приложения MacOS в пакете набора
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ba9dcf62c94d316f404a56c71165357aa3c35a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732004"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="9cafe-103">Тип ресурса Макослобчилдапп</span><span class="sxs-lookup"><span data-stu-id="9cafe-103">macOSLobChildApp resource type</span></span>

<span data-ttu-id="9cafe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cafe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cafe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cafe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cafe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cafe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cafe-107">Содержит свойства бизнес-приложения MacOS в пакете набора</span><span class="sxs-lookup"><span data-stu-id="9cafe-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="9cafe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cafe-108">Properties</span></span>
|<span data-ttu-id="9cafe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cafe-109">Property</span></span>|<span data-ttu-id="9cafe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9cafe-110">Type</span></span>|<span data-ttu-id="9cafe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9cafe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cafe-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="9cafe-112">bundleId</span></span>|<span data-ttu-id="9cafe-113">String</span><span class="sxs-lookup"><span data-stu-id="9cafe-113">String</span></span>|<span data-ttu-id="9cafe-114">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9cafe-114">The Identity Name.</span></span>|
|<span data-ttu-id="9cafe-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9cafe-115">buildNumber</span></span>|<span data-ttu-id="9cafe-116">String</span><span class="sxs-lookup"><span data-stu-id="9cafe-116">String</span></span>|<span data-ttu-id="9cafe-117">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="9cafe-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9cafe-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9cafe-118">versionNumber</span></span>|<span data-ttu-id="9cafe-119">String</span><span class="sxs-lookup"><span data-stu-id="9cafe-119">String</span></span>|<span data-ttu-id="9cafe-120">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="9cafe-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cafe-121">Связи</span><span class="sxs-lookup"><span data-stu-id="9cafe-121">Relationships</span></span>
<span data-ttu-id="9cafe-122">Нет</span><span class="sxs-lookup"><span data-stu-id="9cafe-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cafe-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cafe-123">JSON Representation</span></span>
<span data-ttu-id="9cafe-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cafe-124">Here is a JSON representation of the resource.</span></span>
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





