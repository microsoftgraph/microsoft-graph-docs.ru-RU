---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 38ebee60ad5e4de642103a4cd72ae4f6cea0d9c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031481"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="9448c-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="9448c-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="9448c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9448c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9448c-105">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="9448c-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="9448c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9448c-106">Properties</span></span>
|<span data-ttu-id="9448c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9448c-107">Property</span></span>|<span data-ttu-id="9448c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9448c-108">Type</span></span>|<span data-ttu-id="9448c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9448c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9448c-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="9448c-110">bundleID</span></span>|<span data-ttu-id="9448c-111">String</span><span class="sxs-lookup"><span data-stu-id="9448c-111">String</span></span>|<span data-ttu-id="9448c-112">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="9448c-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="9448c-113">appName</span><span class="sxs-lookup"><span data-stu-id="9448c-113">appName</span></span>|<span data-ttu-id="9448c-114">String</span><span class="sxs-lookup"><span data-stu-id="9448c-114">String</span></span>|<span data-ttu-id="9448c-115">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="9448c-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="9448c-116">publisher</span><span class="sxs-lookup"><span data-stu-id="9448c-116">publisher</span></span>|<span data-ttu-id="9448c-117">String</span><span class="sxs-lookup"><span data-stu-id="9448c-117">String</span></span>|<span data-ttu-id="9448c-118">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="9448c-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="9448c-119">enabled</span><span class="sxs-lookup"><span data-stu-id="9448c-119">enabled</span></span>|<span data-ttu-id="9448c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="9448c-120">Boolean</span></span>|<span data-ttu-id="9448c-121">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9448c-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="9448c-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="9448c-122">showInNotificationCenter</span></span>|<span data-ttu-id="9448c-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9448c-123">Boolean</span></span>|<span data-ttu-id="9448c-124">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="9448c-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="9448c-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="9448c-125">showOnLockScreen</span></span>|<span data-ttu-id="9448c-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9448c-126">Boolean</span></span>|<span data-ttu-id="9448c-127">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="9448c-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="9448c-128">alertType</span><span class="sxs-lookup"><span data-stu-id="9448c-128">alertType</span></span>|[<span data-ttu-id="9448c-129">Иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="9448c-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="9448c-130">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9448c-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="9448c-131">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="9448c-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="9448c-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="9448c-132">badgesEnabled</span></span>|<span data-ttu-id="9448c-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="9448c-133">Boolean</span></span>|<span data-ttu-id="9448c-134">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9448c-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="9448c-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="9448c-135">soundsEnabled</span></span>|<span data-ttu-id="9448c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="9448c-136">Boolean</span></span>|<span data-ttu-id="9448c-137">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9448c-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9448c-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="9448c-138">Relationships</span></span>
<span data-ttu-id="9448c-139">Нет</span><span class="sxs-lookup"><span data-stu-id="9448c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9448c-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9448c-140">JSON Representation</span></span>
<span data-ttu-id="9448c-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9448c-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



