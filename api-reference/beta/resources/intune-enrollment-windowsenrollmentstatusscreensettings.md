---
title: Тип ресурса Виндовсенроллментстатусскринсеттингс
description: Настройка экрана состояния регистрации
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3758dd850a5c98ea2c0ddad4d261fc9a7388ac3c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528227"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="a4494-103">Тип ресурса Виндовсенроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="a4494-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

<span data-ttu-id="a4494-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a4494-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4494-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4494-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4494-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4494-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4494-107">Настройка экрана состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="a4494-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="a4494-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4494-108">Properties</span></span>
|<span data-ttu-id="a4494-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4494-109">Property</span></span>|<span data-ttu-id="a4494-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a4494-110">Type</span></span>|<span data-ttu-id="a4494-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4494-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4494-112">хидеинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="a4494-112">hideInstallationProgress</span></span>|<span data-ttu-id="a4494-113">Логический</span><span class="sxs-lookup"><span data-stu-id="a4494-113">Boolean</span></span>|<span data-ttu-id="a4494-114">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="a4494-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="a4494-115">алловдевицеусебефорепрофилеандаппинсталлкомплете</span><span class="sxs-lookup"><span data-stu-id="a4494-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="a4494-116">Логический</span><span class="sxs-lookup"><span data-stu-id="a4494-116">Boolean</span></span>|<span data-ttu-id="a4494-117">Разрешить или запретить пользователю использовать устройство до завершения установки профилей и приложений</span><span class="sxs-lookup"><span data-stu-id="a4494-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="a4494-118">блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="a4494-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="a4494-119">Логический</span><span class="sxs-lookup"><span data-stu-id="a4494-119">Boolean</span></span>|<span data-ttu-id="a4494-120">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="a4494-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="a4494-121">алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="a4494-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="a4494-122">Логический</span><span class="sxs-lookup"><span data-stu-id="a4494-122">Boolean</span></span>|<span data-ttu-id="a4494-123">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="a4494-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="a4494-124">кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="a4494-124">customErrorMessage</span></span>|<span data-ttu-id="a4494-125">String</span><span class="sxs-lookup"><span data-stu-id="a4494-125">String</span></span>|<span data-ttu-id="a4494-126">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="a4494-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="a4494-127">инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="a4494-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="a4494-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a4494-128">Int32</span></span>|<span data-ttu-id="a4494-129">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="a4494-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="a4494-130">алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="a4494-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="a4494-131">Логический</span><span class="sxs-lookup"><span data-stu-id="a4494-131">Boolean</span></span>|<span data-ttu-id="a4494-132">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="a4494-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4494-133">Связи</span><span class="sxs-lookup"><span data-stu-id="a4494-133">Relationships</span></span>
<span data-ttu-id="a4494-134">Нет</span><span class="sxs-lookup"><span data-stu-id="a4494-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4494-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4494-135">JSON Representation</span></span>
<span data-ttu-id="a4494-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4494-136">Here is a JSON representation of the resource.</span></span>
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



