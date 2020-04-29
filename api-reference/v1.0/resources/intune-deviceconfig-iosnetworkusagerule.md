---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab6f070457db8499caa6f9bb842078086e33c02a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410562"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="0e1b8-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="0e1b8-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="0e1b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e1b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e1b8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e1b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e1b8-106">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="0e1b8-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="0e1b8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e1b8-107">Properties</span></span>
|<span data-ttu-id="0e1b8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e1b8-108">Property</span></span>|<span data-ttu-id="0e1b8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0e1b8-109">Type</span></span>|<span data-ttu-id="0e1b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0e1b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e1b8-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="0e1b8-111">managedApps</span></span>|<span data-ttu-id="0e1b8-112">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="0e1b8-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0e1b8-113">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="0e1b8-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="0e1b8-114">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0e1b8-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0e1b8-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="0e1b8-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="0e1b8-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e1b8-116">Boolean</span></span>|<span data-ttu-id="0e1b8-117">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="0e1b8-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="0e1b8-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="0e1b8-118">cellularDataBlocked</span></span>|<span data-ttu-id="0e1b8-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e1b8-119">Boolean</span></span>|<span data-ttu-id="0e1b8-120">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="0e1b8-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e1b8-121">Связи</span><span class="sxs-lookup"><span data-stu-id="0e1b8-121">Relationships</span></span>
<span data-ttu-id="0e1b8-122">Нет</span><span class="sxs-lookup"><span data-stu-id="0e1b8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e1b8-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e1b8-123">JSON Representation</span></span>
<span data-ttu-id="0e1b8-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e1b8-124">Here is a JSON representation of the resource.</span></span>
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







