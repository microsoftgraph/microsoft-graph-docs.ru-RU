---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0503d938860798408fa5eb2af20ac51dc988f8a7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946450"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="1a73c-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="1a73c-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="1a73c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a73c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a73c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a73c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a73c-106">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1a73c-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="1a73c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a73c-107">Properties</span></span>
|<span data-ttu-id="1a73c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a73c-108">Property</span></span>|<span data-ttu-id="1a73c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1a73c-109">Type</span></span>|<span data-ttu-id="1a73c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a73c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a73c-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="1a73c-111">bundleID</span></span>|<span data-ttu-id="1a73c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="1a73c-112">String</span></span>|<span data-ttu-id="1a73c-113">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1a73c-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="1a73c-114">appName</span><span class="sxs-lookup"><span data-stu-id="1a73c-114">appName</span></span>|<span data-ttu-id="1a73c-115">String</span><span class="sxs-lookup"><span data-stu-id="1a73c-115">String</span></span>|<span data-ttu-id="1a73c-116">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="1a73c-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="1a73c-117">publisher</span><span class="sxs-lookup"><span data-stu-id="1a73c-117">publisher</span></span>|<span data-ttu-id="1a73c-118">String</span><span class="sxs-lookup"><span data-stu-id="1a73c-118">String</span></span>|<span data-ttu-id="1a73c-119">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="1a73c-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="1a73c-120">enabled</span><span class="sxs-lookup"><span data-stu-id="1a73c-120">enabled</span></span>|<span data-ttu-id="1a73c-121">Логический</span><span class="sxs-lookup"><span data-stu-id="1a73c-121">Boolean</span></span>|<span data-ttu-id="1a73c-122">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="1a73c-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="1a73c-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="1a73c-123">showInNotificationCenter</span></span>|<span data-ttu-id="1a73c-124">Логический</span><span class="sxs-lookup"><span data-stu-id="1a73c-124">Boolean</span></span>|<span data-ttu-id="1a73c-125">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1a73c-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="1a73c-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="1a73c-126">showOnLockScreen</span></span>|<span data-ttu-id="1a73c-127">Логический</span><span class="sxs-lookup"><span data-stu-id="1a73c-127">Boolean</span></span>|<span data-ttu-id="1a73c-128">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="1a73c-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="1a73c-129">alertType</span><span class="sxs-lookup"><span data-stu-id="1a73c-129">alertType</span></span>|[<span data-ttu-id="1a73c-130">Иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="1a73c-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="1a73c-131">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="1a73c-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="1a73c-132">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="1a73c-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="1a73c-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="1a73c-133">badgesEnabled</span></span>|<span data-ttu-id="1a73c-134">Логический</span><span class="sxs-lookup"><span data-stu-id="1a73c-134">Boolean</span></span>|<span data-ttu-id="1a73c-135">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="1a73c-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="1a73c-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="1a73c-136">soundsEnabled</span></span>|<span data-ttu-id="1a73c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a73c-137">Boolean</span></span>|<span data-ttu-id="1a73c-138">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="1a73c-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a73c-139">Связи</span><span class="sxs-lookup"><span data-stu-id="1a73c-139">Relationships</span></span>
<span data-ttu-id="1a73c-140">Нет</span><span class="sxs-lookup"><span data-stu-id="1a73c-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a73c-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a73c-141">JSON Representation</span></span>
<span data-ttu-id="1a73c-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a73c-142">Here is a JSON representation of the resource.</span></span>
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




