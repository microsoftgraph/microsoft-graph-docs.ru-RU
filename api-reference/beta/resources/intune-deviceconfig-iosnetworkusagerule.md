---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
localization_priority: Normal
ms.openlocfilehash: 6cf2f0cd88c25a625b12b3adcaac6ccc366ea0e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861000"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="652f5-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="652f5-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="652f5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="652f5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="652f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="652f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="652f5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="652f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="652f5-107">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="652f5-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="652f5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="652f5-108">Properties</span></span>
|<span data-ttu-id="652f5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="652f5-109">Property</span></span>|<span data-ttu-id="652f5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="652f5-110">Type</span></span>|<span data-ttu-id="652f5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="652f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="652f5-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="652f5-112">managedApps</span></span>|<span data-ttu-id="652f5-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="652f5-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="652f5-114">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="652f5-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="652f5-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="652f5-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="652f5-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="652f5-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="652f5-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="652f5-117">Boolean</span></span>|<span data-ttu-id="652f5-118">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="652f5-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="652f5-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="652f5-119">cellularDataBlocked</span></span>|<span data-ttu-id="652f5-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="652f5-120">Boolean</span></span>|<span data-ttu-id="652f5-121">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="652f5-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="652f5-122">Связи</span><span class="sxs-lookup"><span data-stu-id="652f5-122">Relationships</span></span>
<span data-ttu-id="652f5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="652f5-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="652f5-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="652f5-124">JSON Representation</span></span>
<span data-ttu-id="652f5-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="652f5-125">Here is a JSON representation of the resource.</span></span>
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





