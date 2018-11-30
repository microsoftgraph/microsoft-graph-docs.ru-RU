---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
ms.openlocfilehash: 211cbc52f596bbe62647a14c84bd5fd5178fdfc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028160"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="a29fb-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="a29fb-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="a29fb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a29fb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a29fb-105">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="a29fb-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="a29fb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a29fb-106">Properties</span></span>
|<span data-ttu-id="a29fb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a29fb-107">Property</span></span>|<span data-ttu-id="a29fb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a29fb-108">Type</span></span>|<span data-ttu-id="a29fb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a29fb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a29fb-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="a29fb-110">managedApps</span></span>|<span data-ttu-id="a29fb-111">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a29fb-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a29fb-112">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="a29fb-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="a29fb-113">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a29fb-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a29fb-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="a29fb-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="a29fb-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="a29fb-115">Boolean</span></span>|<span data-ttu-id="a29fb-116">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="a29fb-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="a29fb-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="a29fb-117">cellularDataBlocked</span></span>|<span data-ttu-id="a29fb-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="a29fb-118">Boolean</span></span>|<span data-ttu-id="a29fb-119">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="a29fb-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a29fb-120">Связи</span><span class="sxs-lookup"><span data-stu-id="a29fb-120">Relationships</span></span>
<span data-ttu-id="a29fb-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a29fb-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a29fb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a29fb-122">JSON Representation</span></span>
<span data-ttu-id="a29fb-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a29fb-123">Here is a JSON representation of the resource.</span></span>
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



