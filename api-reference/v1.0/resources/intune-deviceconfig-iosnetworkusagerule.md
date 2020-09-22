---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0698ada0fbda3c30e0c2d836c0e949b742b1c99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091693"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="623a9-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="623a9-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="623a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="623a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="623a9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="623a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="623a9-106">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="623a9-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="623a9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="623a9-107">Properties</span></span>
|<span data-ttu-id="623a9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="623a9-108">Property</span></span>|<span data-ttu-id="623a9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="623a9-109">Type</span></span>|<span data-ttu-id="623a9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="623a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623a9-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="623a9-111">managedApps</span></span>|<span data-ttu-id="623a9-112">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="623a9-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="623a9-113">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="623a9-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="623a9-114">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="623a9-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="623a9-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="623a9-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="623a9-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="623a9-116">Boolean</span></span>|<span data-ttu-id="623a9-117">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="623a9-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="623a9-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="623a9-118">cellularDataBlocked</span></span>|<span data-ttu-id="623a9-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="623a9-119">Boolean</span></span>|<span data-ttu-id="623a9-120">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="623a9-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="623a9-121">Связи</span><span class="sxs-lookup"><span data-stu-id="623a9-121">Relationships</span></span>
<span data-ttu-id="623a9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="623a9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="623a9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="623a9-123">JSON Representation</span></span>
<span data-ttu-id="623a9-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="623a9-124">Here is a JSON representation of the resource.</span></span>
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









