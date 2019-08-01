---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9b173a819015901c531bc1fa9632ec906f73d09c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031502"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="2989d-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="2989d-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="2989d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2989d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2989d-105">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="2989d-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="2989d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2989d-106">Properties</span></span>
|<span data-ttu-id="2989d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2989d-107">Property</span></span>|<span data-ttu-id="2989d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2989d-108">Type</span></span>|<span data-ttu-id="2989d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2989d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2989d-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="2989d-110">managedApps</span></span>|<span data-ttu-id="2989d-111">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2989d-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2989d-112">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="2989d-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="2989d-113">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2989d-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="2989d-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="2989d-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="2989d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2989d-115">Boolean</span></span>|<span data-ttu-id="2989d-116">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="2989d-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="2989d-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="2989d-117">cellularDataBlocked</span></span>|<span data-ttu-id="2989d-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="2989d-118">Boolean</span></span>|<span data-ttu-id="2989d-119">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="2989d-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2989d-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="2989d-120">Relationships</span></span>
<span data-ttu-id="2989d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2989d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2989d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2989d-122">JSON Representation</span></span>
<span data-ttu-id="2989d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2989d-123">Here is a JSON representation of the resource.</span></span>
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



