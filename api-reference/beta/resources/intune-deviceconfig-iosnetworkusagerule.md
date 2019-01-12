---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 7476f49c6049eb18e56fa57310aa75707f566bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912024"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="9eb92-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="9eb92-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="9eb92-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9eb92-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9eb92-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eb92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9eb92-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9eb92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9eb92-107">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="9eb92-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="9eb92-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9eb92-108">Properties</span></span>
|<span data-ttu-id="9eb92-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9eb92-109">Property</span></span>|<span data-ttu-id="9eb92-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9eb92-110">Type</span></span>|<span data-ttu-id="9eb92-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9eb92-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9eb92-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="9eb92-112">managedApps</span></span>|<span data-ttu-id="9eb92-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9eb92-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9eb92-114">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="9eb92-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="9eb92-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9eb92-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9eb92-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="9eb92-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="9eb92-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eb92-117">Boolean</span></span>|<span data-ttu-id="9eb92-118">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="9eb92-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="9eb92-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="9eb92-119">cellularDataBlocked</span></span>|<span data-ttu-id="9eb92-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="9eb92-120">Boolean</span></span>|<span data-ttu-id="9eb92-121">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="9eb92-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9eb92-122">Связи</span><span class="sxs-lookup"><span data-stu-id="9eb92-122">Relationships</span></span>
<span data-ttu-id="9eb92-123">Нет</span><span class="sxs-lookup"><span data-stu-id="9eb92-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9eb92-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9eb92-124">JSON Representation</span></span>
<span data-ttu-id="9eb92-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9eb92-125">Here is a JSON representation of the resource.</span></span>
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





