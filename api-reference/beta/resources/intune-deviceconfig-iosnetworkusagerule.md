---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7d11b8a7591d2fce03b3f8a023e9ef90fab4f1b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946926"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="d0360-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="d0360-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="d0360-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0360-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0360-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0360-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0360-106">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="d0360-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="d0360-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0360-107">Properties</span></span>
|<span data-ttu-id="d0360-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0360-108">Property</span></span>|<span data-ttu-id="d0360-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0360-109">Type</span></span>|<span data-ttu-id="d0360-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0360-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0360-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="d0360-111">managedApps</span></span>|<span data-ttu-id="d0360-112">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d0360-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d0360-113">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="d0360-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="d0360-114">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d0360-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d0360-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="d0360-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="d0360-116">Логический</span><span class="sxs-lookup"><span data-stu-id="d0360-116">Boolean</span></span>|<span data-ttu-id="d0360-117">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="d0360-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="d0360-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="d0360-118">cellularDataBlocked</span></span>|<span data-ttu-id="d0360-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0360-119">Boolean</span></span>|<span data-ttu-id="d0360-120">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="d0360-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0360-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d0360-121">Relationships</span></span>
<span data-ttu-id="d0360-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d0360-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0360-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0360-123">JSON Representation</span></span>
<span data-ttu-id="d0360-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0360-124">Here is a JSON representation of the resource.</span></span>
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




