---
title: Тип ресурса Иосаваилаблеупдатеверсион
description: сведения о доступных версиях обновлений iOS
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29cf7500bc7069af0b2a1184adb0fe28bb0ac891
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766366"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="c89cc-103">Тип ресурса Иосаваилаблеупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="c89cc-103">iosAvailableUpdateVersion resource type</span></span>

> <span data-ttu-id="c89cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c89cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c89cc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c89cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c89cc-106">сведения о доступных версиях обновлений iOS</span><span class="sxs-lookup"><span data-stu-id="c89cc-106">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="c89cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c89cc-107">Properties</span></span>
|<span data-ttu-id="c89cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c89cc-108">Property</span></span>|<span data-ttu-id="c89cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c89cc-109">Type</span></span>|<span data-ttu-id="c89cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c89cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c89cc-111">productVersion</span><span class="sxs-lookup"><span data-stu-id="c89cc-111">productVersion</span></span>|<span data-ttu-id="c89cc-112">String</span><span class="sxs-lookup"><span data-stu-id="c89cc-112">String</span></span>|<span data-ttu-id="c89cc-113">Версия обновления.</span><span class="sxs-lookup"><span data-stu-id="c89cc-113">The version of the update.</span></span>|
|<span data-ttu-id="c89cc-114">постингдатетиме</span><span class="sxs-lookup"><span data-stu-id="c89cc-114">postingDateTime</span></span>|<span data-ttu-id="c89cc-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c89cc-115">DateTimeOffset</span></span>|<span data-ttu-id="c89cc-116">Дата разноски обновления.</span><span class="sxs-lookup"><span data-stu-id="c89cc-116">The posting date of the update.</span></span>|
|<span data-ttu-id="c89cc-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c89cc-117">expirationDateTime</span></span>|<span data-ttu-id="c89cc-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c89cc-118">DateTimeOffset</span></span>|<span data-ttu-id="c89cc-119">Дата окончания срока действия обновления.</span><span class="sxs-lookup"><span data-stu-id="c89cc-119">The expiration date of the update.</span></span>|
|<span data-ttu-id="c89cc-120">суппортеддевицес</span><span class="sxs-lookup"><span data-stu-id="c89cc-120">supportedDevices</span></span>|<span data-ttu-id="c89cc-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c89cc-121">String collection</span></span>|<span data-ttu-id="c89cc-122">Список поддерживаемых устройств для обновления.</span><span class="sxs-lookup"><span data-stu-id="c89cc-122">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c89cc-123">Связи</span><span class="sxs-lookup"><span data-stu-id="c89cc-123">Relationships</span></span>
<span data-ttu-id="c89cc-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c89cc-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c89cc-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c89cc-125">JSON Representation</span></span>
<span data-ttu-id="c89cc-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c89cc-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "productVersion": "String",
  "postingDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "supportedDevices": [
    "String"
  ]
}
```



