---
title: Тип ресурса Иосаваилаблеупдатеверсион
description: сведения о доступных версиях обновлений iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3997ce86c780713849d0e0e4773457ff665b0e0d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255604"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="0f18b-103">Тип ресурса Иосаваилаблеупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="0f18b-103">iosAvailableUpdateVersion resource type</span></span>

<span data-ttu-id="0f18b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f18b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f18b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f18b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f18b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f18b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f18b-107">сведения о доступных версиях обновлений iOS</span><span class="sxs-lookup"><span data-stu-id="0f18b-107">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="0f18b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f18b-108">Properties</span></span>
|<span data-ttu-id="0f18b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f18b-109">Property</span></span>|<span data-ttu-id="0f18b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f18b-110">Type</span></span>|<span data-ttu-id="0f18b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f18b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f18b-112">productVersion</span><span class="sxs-lookup"><span data-stu-id="0f18b-112">productVersion</span></span>|<span data-ttu-id="0f18b-113">String</span><span class="sxs-lookup"><span data-stu-id="0f18b-113">String</span></span>|<span data-ttu-id="0f18b-114">Версия обновления.</span><span class="sxs-lookup"><span data-stu-id="0f18b-114">The version of the update.</span></span>|
|<span data-ttu-id="0f18b-115">постингдатетиме</span><span class="sxs-lookup"><span data-stu-id="0f18b-115">postingDateTime</span></span>|<span data-ttu-id="0f18b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f18b-116">DateTimeOffset</span></span>|<span data-ttu-id="0f18b-117">Дата разноски обновления.</span><span class="sxs-lookup"><span data-stu-id="0f18b-117">The posting date of the update.</span></span>|
|<span data-ttu-id="0f18b-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0f18b-118">expirationDateTime</span></span>|<span data-ttu-id="0f18b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f18b-119">DateTimeOffset</span></span>|<span data-ttu-id="0f18b-120">Дата окончания срока действия обновления.</span><span class="sxs-lookup"><span data-stu-id="0f18b-120">The expiration date of the update.</span></span>|
|<span data-ttu-id="0f18b-121">суппортеддевицес</span><span class="sxs-lookup"><span data-stu-id="0f18b-121">supportedDevices</span></span>|<span data-ttu-id="0f18b-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0f18b-122">String collection</span></span>|<span data-ttu-id="0f18b-123">Список поддерживаемых устройств для обновления.</span><span class="sxs-lookup"><span data-stu-id="0f18b-123">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f18b-124">Связи</span><span class="sxs-lookup"><span data-stu-id="0f18b-124">Relationships</span></span>
<span data-ttu-id="0f18b-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0f18b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f18b-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f18b-126">JSON Representation</span></span>
<span data-ttu-id="0f18b-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f18b-127">Here is a JSON representation of the resource.</span></span>
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




