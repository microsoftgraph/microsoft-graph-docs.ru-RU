---
title: Тип ресурса Виндовсенроллментстатусскринсеттингс
description: Настройка экрана состояния регистрации
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b47d24b7bec3b20b23077e34b36a9f9e95387789
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358133"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="6ae01-103">Тип ресурса Виндовсенроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="6ae01-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

<span data-ttu-id="6ae01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ae01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ae01-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ae01-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ae01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ae01-107">Настройка экрана состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="6ae01-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="6ae01-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ae01-108">Properties</span></span>
|<span data-ttu-id="6ae01-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ae01-109">Property</span></span>|<span data-ttu-id="6ae01-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6ae01-110">Type</span></span>|<span data-ttu-id="6ae01-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6ae01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ae01-112">хидеинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="6ae01-112">hideInstallationProgress</span></span>|<span data-ttu-id="6ae01-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae01-113">Boolean</span></span>|<span data-ttu-id="6ae01-114">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="6ae01-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="6ae01-115">алловдевицеусебефорепрофилеандаппинсталлкомплете</span><span class="sxs-lookup"><span data-stu-id="6ae01-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="6ae01-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae01-116">Boolean</span></span>|<span data-ttu-id="6ae01-117">Разрешить или запретить пользователю использовать устройство до завершения установки профилей и приложений</span><span class="sxs-lookup"><span data-stu-id="6ae01-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="6ae01-118">блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="6ae01-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="6ae01-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae01-119">Boolean</span></span>|<span data-ttu-id="6ae01-120">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="6ae01-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="6ae01-121">алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="6ae01-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="6ae01-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae01-122">Boolean</span></span>|<span data-ttu-id="6ae01-123">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="6ae01-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="6ae01-124">кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="6ae01-124">customErrorMessage</span></span>|<span data-ttu-id="6ae01-125">String</span><span class="sxs-lookup"><span data-stu-id="6ae01-125">String</span></span>|<span data-ttu-id="6ae01-126">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="6ae01-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="6ae01-127">инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="6ae01-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="6ae01-128">Int32</span><span class="sxs-lookup"><span data-stu-id="6ae01-128">Int32</span></span>|<span data-ttu-id="6ae01-129">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="6ae01-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="6ae01-130">алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="6ae01-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="6ae01-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae01-131">Boolean</span></span>|<span data-ttu-id="6ae01-132">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="6ae01-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ae01-133">Связи</span><span class="sxs-lookup"><span data-stu-id="6ae01-133">Relationships</span></span>
<span data-ttu-id="6ae01-134">Нет</span><span class="sxs-lookup"><span data-stu-id="6ae01-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ae01-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ae01-135">JSON Representation</span></span>
<span data-ttu-id="6ae01-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ae01-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```



