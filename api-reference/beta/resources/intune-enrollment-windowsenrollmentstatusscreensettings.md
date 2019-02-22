---
title: Тип ресурса Виндовсенроллментстатусскринсеттингс
description: Настройка экрана состояния регистрации
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5684a447b82f285784eda1bf71c13f35d766a570
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148687"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="7089c-103">Тип ресурса Виндовсенроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="7089c-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="7089c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7089c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7089c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7089c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7089c-106">Настройка экрана состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="7089c-106">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="7089c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7089c-107">Properties</span></span>
|<span data-ttu-id="7089c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7089c-108">Property</span></span>|<span data-ttu-id="7089c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7089c-109">Type</span></span>|<span data-ttu-id="7089c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7089c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7089c-111">Хидеинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="7089c-111">hideInstallationProgress</span></span>|<span data-ttu-id="7089c-112">Логический</span><span class="sxs-lookup"><span data-stu-id="7089c-112">Boolean</span></span>|<span data-ttu-id="7089c-113">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="7089c-113">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="7089c-114">Алловдевицеусебефорепрофилеандаппинсталлкомплете</span><span class="sxs-lookup"><span data-stu-id="7089c-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="7089c-115">Логический</span><span class="sxs-lookup"><span data-stu-id="7089c-115">Boolean</span></span>|<span data-ttu-id="7089c-116">Разрешить или запретить пользователю использовать устройство до завершения установки профилей и приложений</span><span class="sxs-lookup"><span data-stu-id="7089c-116">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="7089c-117">Блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="7089c-117">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="7089c-118">Логический</span><span class="sxs-lookup"><span data-stu-id="7089c-118">Boolean</span></span>|<span data-ttu-id="7089c-119">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="7089c-119">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="7089c-120">Алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="7089c-120">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="7089c-121">Логический</span><span class="sxs-lookup"><span data-stu-id="7089c-121">Boolean</span></span>|<span data-ttu-id="7089c-122">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="7089c-122">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="7089c-123">Кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="7089c-123">customErrorMessage</span></span>|<span data-ttu-id="7089c-124">String</span><span class="sxs-lookup"><span data-stu-id="7089c-124">String</span></span>|<span data-ttu-id="7089c-125">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="7089c-125">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="7089c-126">Инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="7089c-126">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="7089c-127">Int32</span><span class="sxs-lookup"><span data-stu-id="7089c-127">Int32</span></span>|<span data-ttu-id="7089c-128">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="7089c-128">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="7089c-129">Алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="7089c-129">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="7089c-130">Логический</span><span class="sxs-lookup"><span data-stu-id="7089c-130">Boolean</span></span>|<span data-ttu-id="7089c-131">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="7089c-131">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="7089c-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="7089c-132">Relationships</span></span>
<span data-ttu-id="7089c-133">Нет</span><span class="sxs-lookup"><span data-stu-id="7089c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7089c-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7089c-134">JSON Representation</span></span>
<span data-ttu-id="7089c-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7089c-135">Here is a JSON representation of the resource.</span></span>
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




