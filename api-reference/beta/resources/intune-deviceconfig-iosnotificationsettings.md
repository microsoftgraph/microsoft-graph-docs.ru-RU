---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ca6c5cf968897d701870bc695dcce909c74f1fc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280139"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="a3cf2-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="a3cf2-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="a3cf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3cf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3cf2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3cf2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3cf2-107">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="a3cf2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3cf2-108">Properties</span></span>
|<span data-ttu-id="a3cf2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3cf2-109">Property</span></span>|<span data-ttu-id="a3cf2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a3cf2-110">Type</span></span>|<span data-ttu-id="a3cf2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a3cf2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3cf2-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="a3cf2-112">bundleID</span></span>|<span data-ttu-id="a3cf2-113">String</span><span class="sxs-lookup"><span data-stu-id="a3cf2-113">String</span></span>|<span data-ttu-id="a3cf2-114">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="a3cf2-115">appName</span><span class="sxs-lookup"><span data-stu-id="a3cf2-115">appName</span></span>|<span data-ttu-id="a3cf2-116">String</span><span class="sxs-lookup"><span data-stu-id="a3cf2-116">String</span></span>|<span data-ttu-id="a3cf2-117">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="a3cf2-118">publisher</span><span class="sxs-lookup"><span data-stu-id="a3cf2-118">publisher</span></span>|<span data-ttu-id="a3cf2-119">String</span><span class="sxs-lookup"><span data-stu-id="a3cf2-119">String</span></span>|<span data-ttu-id="a3cf2-120">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="a3cf2-121">enabled</span><span class="sxs-lookup"><span data-stu-id="a3cf2-121">enabled</span></span>|<span data-ttu-id="a3cf2-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cf2-122">Boolean</span></span>|<span data-ttu-id="a3cf2-123">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="a3cf2-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="a3cf2-124">showInNotificationCenter</span></span>|<span data-ttu-id="a3cf2-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cf2-125">Boolean</span></span>|<span data-ttu-id="a3cf2-126">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="a3cf2-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="a3cf2-127">showOnLockScreen</span></span>|<span data-ttu-id="a3cf2-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cf2-128">Boolean</span></span>|<span data-ttu-id="a3cf2-129">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="a3cf2-130">alertType</span><span class="sxs-lookup"><span data-stu-id="a3cf2-130">alertType</span></span>|[<span data-ttu-id="a3cf2-131">иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="a3cf2-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="a3cf2-132">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="a3cf2-133">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="a3cf2-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="a3cf2-134">badgesEnabled</span></span>|<span data-ttu-id="a3cf2-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cf2-135">Boolean</span></span>|<span data-ttu-id="a3cf2-136">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="a3cf2-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="a3cf2-137">soundsEnabled</span></span>|<span data-ttu-id="a3cf2-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cf2-138">Boolean</span></span>|<span data-ttu-id="a3cf2-139">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-139">Indicates whether sounds are allowed for this app.</span></span>|
|<span data-ttu-id="a3cf2-140">превиеввисибилити</span><span class="sxs-lookup"><span data-stu-id="a3cf2-140">previewVisibility</span></span>|[<span data-ttu-id="a3cf2-141">иоснотификатионпревиеввисибилити</span><span class="sxs-lookup"><span data-stu-id="a3cf2-141">iosNotificationPreviewVisibility</span></span>](../resources/intune-deviceconfig-iosnotificationpreviewvisibility.md)|<span data-ttu-id="a3cf2-142">Переопределяет политику просмотра уведомлений, установленную пользователем на устройстве с iOS.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-142">Overrides the notification preview policy set by the user on an iOS device.</span></span> <span data-ttu-id="a3cf2-143">Возможные значения: `notConfigured`, `alwaysShow`, `hideWhenLocked`, `neverShow`.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-143">Possible values are: `notConfigured`, `alwaysShow`, `hideWhenLocked`, `neverShow`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3cf2-144">Связи</span><span class="sxs-lookup"><span data-stu-id="a3cf2-144">Relationships</span></span>
<span data-ttu-id="a3cf2-145">Нет</span><span class="sxs-lookup"><span data-stu-id="a3cf2-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3cf2-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3cf2-146">JSON Representation</span></span>
<span data-ttu-id="a3cf2-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3cf2-147">Here is a JSON representation of the resource.</span></span>
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
  "soundsEnabled": true,
  "previewVisibility": "String"
}
```




