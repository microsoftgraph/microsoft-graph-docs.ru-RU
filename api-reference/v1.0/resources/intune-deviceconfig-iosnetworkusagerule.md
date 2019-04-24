---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 516e880e4b6230ca165426b849f57609dcc6e6ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585071"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="5d6b2-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="5d6b2-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="5d6b2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d6b2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d6b2-105">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="5d6b2-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="5d6b2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d6b2-106">Properties</span></span>
|<span data-ttu-id="5d6b2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d6b2-107">Property</span></span>|<span data-ttu-id="5d6b2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5d6b2-108">Type</span></span>|<span data-ttu-id="5d6b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5d6b2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d6b2-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="5d6b2-110">managedApps</span></span>|<span data-ttu-id="5d6b2-111">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5d6b2-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5d6b2-112">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="5d6b2-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="5d6b2-113">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5d6b2-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5d6b2-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="5d6b2-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="5d6b2-115">Логический</span><span class="sxs-lookup"><span data-stu-id="5d6b2-115">Boolean</span></span>|<span data-ttu-id="5d6b2-116">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="5d6b2-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="5d6b2-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="5d6b2-117">cellularDataBlocked</span></span>|<span data-ttu-id="5d6b2-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d6b2-118">Boolean</span></span>|<span data-ttu-id="5d6b2-119">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="5d6b2-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d6b2-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="5d6b2-120">Relationships</span></span>
<span data-ttu-id="5d6b2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5d6b2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d6b2-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d6b2-122">JSON Representation</span></span>
<span data-ttu-id="5d6b2-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d6b2-123">Here is a JSON representation of the resource.</span></span>
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



