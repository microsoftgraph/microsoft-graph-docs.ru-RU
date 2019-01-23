---
title: Тип ресурса iosNetworkUsageRule
description: Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a287fcf8be771037a39efd821f5468acf518371
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398326"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="0ad95-103">Тип ресурса iosNetworkUsageRule</span><span class="sxs-lookup"><span data-stu-id="0ad95-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="0ad95-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ad95-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ad95-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ad95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ad95-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ad95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ad95-107">Благодаря правилам использования сети предприятия могут определять, как управляемые приложения используют сети, например мобильные сети.</span><span class="sxs-lookup"><span data-stu-id="0ad95-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="0ad95-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ad95-108">Properties</span></span>
|<span data-ttu-id="0ad95-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ad95-109">Property</span></span>|<span data-ttu-id="0ad95-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0ad95-110">Type</span></span>|<span data-ttu-id="0ad95-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0ad95-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ad95-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="0ad95-112">managedApps</span></span>|<span data-ttu-id="0ad95-113">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ad95-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0ad95-114">Сведения об управляемых приложениях, к которым применяется это правило.</span><span class="sxs-lookup"><span data-stu-id="0ad95-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="0ad95-115">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0ad95-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0ad95-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="0ad95-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="0ad95-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad95-117">Boolean</span></span>|<span data-ttu-id="0ad95-118">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в роуминге.</span><span class="sxs-lookup"><span data-stu-id="0ad95-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="0ad95-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="0ad95-119">cellularDataBlocked</span></span>|<span data-ttu-id="0ad95-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ad95-120">Boolean</span></span>|<span data-ttu-id="0ad95-121">Если задано значение true, соответствующим управляемым приложениям запрещается использовать мобильные данные в любое время.</span><span class="sxs-lookup"><span data-stu-id="0ad95-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ad95-122">Связи</span><span class="sxs-lookup"><span data-stu-id="0ad95-122">Relationships</span></span>
<span data-ttu-id="0ad95-123">Нет</span><span class="sxs-lookup"><span data-stu-id="0ad95-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ad95-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ad95-124">JSON Representation</span></span>
<span data-ttu-id="0ad95-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ad95-125">Here is a JSON representation of the resource.</span></span>
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




