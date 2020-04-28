---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 422600c9bffd6b1e7849cabc30229645cab486e7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440475"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="f5ba8-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="f5ba8-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="f5ba8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ba8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5ba8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5ba8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5ba8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5ba8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5ba8-107">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="f5ba8-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="f5ba8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5ba8-108">Properties</span></span>
|<span data-ttu-id="f5ba8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5ba8-109">Property</span></span>|<span data-ttu-id="f5ba8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f5ba8-110">Type</span></span>|<span data-ttu-id="f5ba8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f5ba8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ba8-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="f5ba8-112">managedApps</span></span>|<span data-ttu-id="f5ba8-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5ba8-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f5ba8-114">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="f5ba8-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="f5ba8-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f5ba8-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f5ba8-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="f5ba8-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="f5ba8-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5ba8-117">Boolean</span></span>|<span data-ttu-id="f5ba8-118">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="f5ba8-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="f5ba8-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="f5ba8-119">cellularDataBlocked</span></span>|<span data-ttu-id="f5ba8-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5ba8-120">Boolean</span></span>|<span data-ttu-id="f5ba8-121">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="f5ba8-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5ba8-122">Связи</span><span class="sxs-lookup"><span data-stu-id="f5ba8-122">Relationships</span></span>
<span data-ttu-id="f5ba8-123">Нет</span><span class="sxs-lookup"><span data-stu-id="f5ba8-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5ba8-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5ba8-124">JSON Representation</span></span>
<span data-ttu-id="f5ba8-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5ba8-125">Here is a JSON representation of the resource.</span></span>
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



