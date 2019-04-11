---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e91940e5d090cc64bd0d98fa5f644b72d7f3a0a7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779897"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="04a63-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="04a63-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="04a63-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04a63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04a63-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04a63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04a63-106">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="04a63-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="04a63-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="04a63-107">Properties</span></span>
|<span data-ttu-id="04a63-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="04a63-108">Property</span></span>|<span data-ttu-id="04a63-109">Тип</span><span class="sxs-lookup"><span data-stu-id="04a63-109">Type</span></span>|<span data-ttu-id="04a63-110">Описание</span><span class="sxs-lookup"><span data-stu-id="04a63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04a63-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="04a63-111">managedApps</span></span>|<span data-ttu-id="04a63-112">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="04a63-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="04a63-113">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="04a63-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="04a63-114">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="04a63-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="04a63-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="04a63-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="04a63-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="04a63-116">Boolean</span></span>|<span data-ttu-id="04a63-117">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="04a63-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="04a63-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="04a63-118">cellularDataBlocked</span></span>|<span data-ttu-id="04a63-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="04a63-119">Boolean</span></span>|<span data-ttu-id="04a63-120">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="04a63-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04a63-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="04a63-121">Relationships</span></span>
<span data-ttu-id="04a63-122">Нет</span><span class="sxs-lookup"><span data-stu-id="04a63-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04a63-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04a63-123">JSON Representation</span></span>
<span data-ttu-id="04a63-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04a63-124">Here is a JSON representation of the resource.</span></span>
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





