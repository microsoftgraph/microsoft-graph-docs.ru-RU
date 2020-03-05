---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99e9f769be7184df600e16544ca19f2c26d56391
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526334"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="5cc39-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="5cc39-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="5cc39-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5cc39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cc39-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cc39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cc39-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5cc39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cc39-107">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="5cc39-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="5cc39-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cc39-108">Properties</span></span>
|<span data-ttu-id="5cc39-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cc39-109">Property</span></span>|<span data-ttu-id="5cc39-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5cc39-110">Type</span></span>|<span data-ttu-id="5cc39-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5cc39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cc39-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="5cc39-112">managedApps</span></span>|<span data-ttu-id="5cc39-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5cc39-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5cc39-114">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="5cc39-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="5cc39-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5cc39-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5cc39-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="5cc39-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="5cc39-117">Логический</span><span class="sxs-lookup"><span data-stu-id="5cc39-117">Boolean</span></span>|<span data-ttu-id="5cc39-118">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="5cc39-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="5cc39-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="5cc39-119">cellularDataBlocked</span></span>|<span data-ttu-id="5cc39-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cc39-120">Boolean</span></span>|<span data-ttu-id="5cc39-121">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="5cc39-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cc39-122">Связи</span><span class="sxs-lookup"><span data-stu-id="5cc39-122">Relationships</span></span>
<span data-ttu-id="5cc39-123">Нет</span><span class="sxs-lookup"><span data-stu-id="5cc39-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cc39-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cc39-124">JSON Representation</span></span>
<span data-ttu-id="5cc39-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cc39-125">Here is a JSON representation of the resource.</span></span>
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



