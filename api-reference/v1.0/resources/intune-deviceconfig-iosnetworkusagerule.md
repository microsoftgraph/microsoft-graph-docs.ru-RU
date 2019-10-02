---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: abe641a0a714c8e2d9e171ccb874905b3a6321b6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359063"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="25e8f-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="25e8f-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="25e8f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25e8f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25e8f-105">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="25e8f-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="25e8f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="25e8f-106">Properties</span></span>
|<span data-ttu-id="25e8f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="25e8f-107">Property</span></span>|<span data-ttu-id="25e8f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="25e8f-108">Type</span></span>|<span data-ttu-id="25e8f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25e8f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25e8f-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="25e8f-110">managedApps</span></span>|<span data-ttu-id="25e8f-111">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="25e8f-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="25e8f-112">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="25e8f-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="25e8f-113">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="25e8f-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="25e8f-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="25e8f-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="25e8f-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="25e8f-115">Boolean</span></span>|<span data-ttu-id="25e8f-116">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="25e8f-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="25e8f-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="25e8f-117">cellularDataBlocked</span></span>|<span data-ttu-id="25e8f-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="25e8f-118">Boolean</span></span>|<span data-ttu-id="25e8f-119">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="25e8f-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25e8f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="25e8f-120">Relationships</span></span>
<span data-ttu-id="25e8f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="25e8f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25e8f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25e8f-122">JSON Representation</span></span>
<span data-ttu-id="25e8f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25e8f-123">Here is a JSON representation of the resource.</span></span>
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




