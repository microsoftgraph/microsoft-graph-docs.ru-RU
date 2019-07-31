---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0d656c7df770c59d0787dcf40ad1081bb8984cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970418"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="4f141-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="4f141-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="4f141-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f141-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f141-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f141-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f141-106">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4f141-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="4f141-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f141-107">Properties</span></span>
|<span data-ttu-id="4f141-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f141-108">Property</span></span>|<span data-ttu-id="4f141-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4f141-109">Type</span></span>|<span data-ttu-id="4f141-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4f141-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f141-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="4f141-111">bundleID</span></span>|<span data-ttu-id="4f141-112">String</span><span class="sxs-lookup"><span data-stu-id="4f141-112">String</span></span>|<span data-ttu-id="4f141-113">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4f141-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="4f141-114">appName</span><span class="sxs-lookup"><span data-stu-id="4f141-114">appName</span></span>|<span data-ttu-id="4f141-115">String</span><span class="sxs-lookup"><span data-stu-id="4f141-115">String</span></span>|<span data-ttu-id="4f141-116">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="4f141-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="4f141-117">publisher</span><span class="sxs-lookup"><span data-stu-id="4f141-117">publisher</span></span>|<span data-ttu-id="4f141-118">String</span><span class="sxs-lookup"><span data-stu-id="4f141-118">String</span></span>|<span data-ttu-id="4f141-119">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="4f141-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="4f141-120">enabled</span><span class="sxs-lookup"><span data-stu-id="4f141-120">enabled</span></span>|<span data-ttu-id="4f141-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f141-121">Boolean</span></span>|<span data-ttu-id="4f141-122">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="4f141-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="4f141-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="4f141-123">showInNotificationCenter</span></span>|<span data-ttu-id="4f141-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f141-124">Boolean</span></span>|<span data-ttu-id="4f141-125">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4f141-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="4f141-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="4f141-126">showOnLockScreen</span></span>|<span data-ttu-id="4f141-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f141-127">Boolean</span></span>|<span data-ttu-id="4f141-128">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="4f141-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="4f141-129">alertType</span><span class="sxs-lookup"><span data-stu-id="4f141-129">alertType</span></span>|[<span data-ttu-id="4f141-130">Иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="4f141-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="4f141-131">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="4f141-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="4f141-132">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="4f141-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="4f141-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="4f141-133">badgesEnabled</span></span>|<span data-ttu-id="4f141-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f141-134">Boolean</span></span>|<span data-ttu-id="4f141-135">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="4f141-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="4f141-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="4f141-136">soundsEnabled</span></span>|<span data-ttu-id="4f141-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f141-137">Boolean</span></span>|<span data-ttu-id="4f141-138">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="4f141-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f141-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="4f141-139">Relationships</span></span>
<span data-ttu-id="4f141-140">Нет</span><span class="sxs-lookup"><span data-stu-id="4f141-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f141-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f141-141">JSON Representation</span></span>
<span data-ttu-id="4f141-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f141-142">Here is a JSON representation of the resource.</span></span>
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





