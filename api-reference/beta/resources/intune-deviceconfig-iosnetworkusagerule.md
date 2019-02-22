---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03cc8c1586bb851d54d9ba87f947b6b6d7b254b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168329"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="7e637-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="7e637-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="7e637-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e637-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e637-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e637-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e637-106">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="7e637-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="7e637-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e637-107">Properties</span></span>
|<span data-ttu-id="7e637-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e637-108">Property</span></span>|<span data-ttu-id="7e637-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7e637-109">Type</span></span>|<span data-ttu-id="7e637-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7e637-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e637-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="7e637-111">managedApps</span></span>|<span data-ttu-id="7e637-112">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7e637-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7e637-113">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="7e637-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="7e637-114">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7e637-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7e637-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="7e637-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="7e637-116">Логический</span><span class="sxs-lookup"><span data-stu-id="7e637-116">Boolean</span></span>|<span data-ttu-id="7e637-117">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="7e637-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="7e637-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="7e637-118">cellularDataBlocked</span></span>|<span data-ttu-id="7e637-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e637-119">Boolean</span></span>|<span data-ttu-id="7e637-120">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="7e637-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e637-121">Связи</span><span class="sxs-lookup"><span data-stu-id="7e637-121">Relationships</span></span>
<span data-ttu-id="7e637-122">Нет</span><span class="sxs-lookup"><span data-stu-id="7e637-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e637-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e637-123">JSON Representation</span></span>
<span data-ttu-id="7e637-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e637-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```




