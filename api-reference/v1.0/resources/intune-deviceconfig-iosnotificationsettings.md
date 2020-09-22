---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e3dc929e96869475d4376c344bf08ff17ae7edd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074988"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="b2c85-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="b2c85-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="b2c85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2c85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2c85-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2c85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2c85-106">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="b2c85-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="b2c85-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2c85-107">Properties</span></span>
|<span data-ttu-id="b2c85-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2c85-108">Property</span></span>|<span data-ttu-id="b2c85-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b2c85-109">Type</span></span>|<span data-ttu-id="b2c85-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2c85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2c85-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="b2c85-111">bundleID</span></span>|<span data-ttu-id="b2c85-112">String</span><span class="sxs-lookup"><span data-stu-id="b2c85-112">String</span></span>|<span data-ttu-id="b2c85-113">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="b2c85-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="b2c85-114">appName</span><span class="sxs-lookup"><span data-stu-id="b2c85-114">appName</span></span>|<span data-ttu-id="b2c85-115">String</span><span class="sxs-lookup"><span data-stu-id="b2c85-115">String</span></span>|<span data-ttu-id="b2c85-116">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="b2c85-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="b2c85-117">publisher</span><span class="sxs-lookup"><span data-stu-id="b2c85-117">publisher</span></span>|<span data-ttu-id="b2c85-118">String</span><span class="sxs-lookup"><span data-stu-id="b2c85-118">String</span></span>|<span data-ttu-id="b2c85-119">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="b2c85-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="b2c85-120">enabled</span><span class="sxs-lookup"><span data-stu-id="b2c85-120">enabled</span></span>|<span data-ttu-id="b2c85-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2c85-121">Boolean</span></span>|<span data-ttu-id="b2c85-122">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="b2c85-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="b2c85-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="b2c85-123">showInNotificationCenter</span></span>|<span data-ttu-id="b2c85-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2c85-124">Boolean</span></span>|<span data-ttu-id="b2c85-125">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="b2c85-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="b2c85-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b2c85-126">showOnLockScreen</span></span>|<span data-ttu-id="b2c85-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2c85-127">Boolean</span></span>|<span data-ttu-id="b2c85-128">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="b2c85-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="b2c85-129">alertType</span><span class="sxs-lookup"><span data-stu-id="b2c85-129">alertType</span></span>|[<span data-ttu-id="b2c85-130">иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="b2c85-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="b2c85-131">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="b2c85-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="b2c85-132">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="b2c85-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="b2c85-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="b2c85-133">badgesEnabled</span></span>|<span data-ttu-id="b2c85-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2c85-134">Boolean</span></span>|<span data-ttu-id="b2c85-135">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="b2c85-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="b2c85-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="b2c85-136">soundsEnabled</span></span>|<span data-ttu-id="b2c85-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2c85-137">Boolean</span></span>|<span data-ttu-id="b2c85-138">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="b2c85-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2c85-139">Связи</span><span class="sxs-lookup"><span data-stu-id="b2c85-139">Relationships</span></span>
<span data-ttu-id="b2c85-140">Нет</span><span class="sxs-lookup"><span data-stu-id="b2c85-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2c85-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2c85-141">JSON Representation</span></span>
<span data-ttu-id="b2c85-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2c85-142">Here is a JSON representation of the resource.</span></span>
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









