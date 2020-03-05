---
title: Тип ресурса Иосаваилаблеупдатеверсион
description: сведения о доступных версиях обновлений iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b2174e13cf80e39e1f63f7fb03da6e9b305add30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523445"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="28c1e-103">Тип ресурса Иосаваилаблеупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="28c1e-103">iosAvailableUpdateVersion resource type</span></span>

<span data-ttu-id="28c1e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="28c1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28c1e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28c1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28c1e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28c1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c1e-107">сведения о доступных версиях обновлений iOS</span><span class="sxs-lookup"><span data-stu-id="28c1e-107">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="28c1e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="28c1e-108">Properties</span></span>
|<span data-ttu-id="28c1e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="28c1e-109">Property</span></span>|<span data-ttu-id="28c1e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="28c1e-110">Type</span></span>|<span data-ttu-id="28c1e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="28c1e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c1e-112">productVersion</span><span class="sxs-lookup"><span data-stu-id="28c1e-112">productVersion</span></span>|<span data-ttu-id="28c1e-113">String</span><span class="sxs-lookup"><span data-stu-id="28c1e-113">String</span></span>|<span data-ttu-id="28c1e-114">Версия обновления.</span><span class="sxs-lookup"><span data-stu-id="28c1e-114">The version of the update.</span></span>|
|<span data-ttu-id="28c1e-115">постингдатетиме</span><span class="sxs-lookup"><span data-stu-id="28c1e-115">postingDateTime</span></span>|<span data-ttu-id="28c1e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28c1e-116">DateTimeOffset</span></span>|<span data-ttu-id="28c1e-117">Дата разноски обновления.</span><span class="sxs-lookup"><span data-stu-id="28c1e-117">The posting date of the update.</span></span>|
|<span data-ttu-id="28c1e-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="28c1e-118">expirationDateTime</span></span>|<span data-ttu-id="28c1e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28c1e-119">DateTimeOffset</span></span>|<span data-ttu-id="28c1e-120">Дата окончания срока действия обновления.</span><span class="sxs-lookup"><span data-stu-id="28c1e-120">The expiration date of the update.</span></span>|
|<span data-ttu-id="28c1e-121">суппортеддевицес</span><span class="sxs-lookup"><span data-stu-id="28c1e-121">supportedDevices</span></span>|<span data-ttu-id="28c1e-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="28c1e-122">String collection</span></span>|<span data-ttu-id="28c1e-123">Список поддерживаемых устройств для обновления.</span><span class="sxs-lookup"><span data-stu-id="28c1e-123">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28c1e-124">Связи</span><span class="sxs-lookup"><span data-stu-id="28c1e-124">Relationships</span></span>
<span data-ttu-id="28c1e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="28c1e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28c1e-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28c1e-126">JSON Representation</span></span>
<span data-ttu-id="28c1e-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28c1e-127">Here is a JSON representation of the resource.</span></span>
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



