---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f273ae6cd6d9b40dd19d65df342c0e83fef61bd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085012"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="a84e1-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="a84e1-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="a84e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a84e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a84e1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a84e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a84e1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a84e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a84e1-107">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="a84e1-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="a84e1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a84e1-108">Properties</span></span>
|<span data-ttu-id="a84e1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a84e1-109">Property</span></span>|<span data-ttu-id="a84e1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a84e1-110">Type</span></span>|<span data-ttu-id="a84e1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a84e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a84e1-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="a84e1-112">managedApps</span></span>|<span data-ttu-id="a84e1-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a84e1-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a84e1-114">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="a84e1-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="a84e1-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a84e1-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a84e1-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="a84e1-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="a84e1-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a84e1-117">Boolean</span></span>|<span data-ttu-id="a84e1-118">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="a84e1-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="a84e1-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="a84e1-119">cellularDataBlocked</span></span>|<span data-ttu-id="a84e1-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a84e1-120">Boolean</span></span>|<span data-ttu-id="a84e1-121">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="a84e1-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a84e1-122">Связи</span><span class="sxs-lookup"><span data-stu-id="a84e1-122">Relationships</span></span>
<span data-ttu-id="a84e1-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a84e1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a84e1-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a84e1-124">JSON Representation</span></span>
<span data-ttu-id="a84e1-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a84e1-125">Here is a JSON representation of the resource.</span></span>
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






