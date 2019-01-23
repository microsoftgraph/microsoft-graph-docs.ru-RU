---
title: Тип ресурса windowsEnrollmentStatusScreenSettings
description: Параметр экрана состояния подачи заявок
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399936"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="7bb0b-103">Тип ресурса windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="7bb0b-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="7bb0b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7bb0b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7bb0b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bb0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bb0b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bb0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bb0b-107">Параметр экрана состояния подачи заявок</span><span class="sxs-lookup"><span data-stu-id="7bb0b-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="7bb0b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bb0b-108">Properties</span></span>
|<span data-ttu-id="7bb0b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bb0b-109">Property</span></span>|<span data-ttu-id="7bb0b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7bb0b-110">Type</span></span>|<span data-ttu-id="7bb0b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7bb0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bb0b-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="7bb0b-112">hideInstallationProgress</span></span>|<span data-ttu-id="7bb0b-113">Логический</span><span class="sxs-lookup"><span data-stu-id="7bb0b-113">Boolean</span></span>|<span data-ttu-id="7bb0b-114">Показать или скрыть выполнения установки для пользователей</span><span class="sxs-lookup"><span data-stu-id="7bb0b-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="7bb0b-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="7bb0b-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="7bb0b-116">Логический</span><span class="sxs-lookup"><span data-stu-id="7bb0b-116">Boolean</span></span>|<span data-ttu-id="7bb0b-117">Разрешить или заблокировать пользователя для использования устройств до завершения установки приложения и профилей</span><span class="sxs-lookup"><span data-stu-id="7bb0b-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="7bb0b-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="7bb0b-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="7bb0b-119">Логический</span><span class="sxs-lookup"><span data-stu-id="7bb0b-119">Boolean</span></span>|<span data-ttu-id="7bb0b-120">Пользователь может повторно запустите программу установки на сбой установки</span><span class="sxs-lookup"><span data-stu-id="7bb0b-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="7bb0b-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7bb0b-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="7bb0b-122">Логический</span><span class="sxs-lookup"><span data-stu-id="7bb0b-122">Boolean</span></span>|<span data-ttu-id="7bb0b-123">Разрешить или заблокировать семейства журнала на сбой установки</span><span class="sxs-lookup"><span data-stu-id="7bb0b-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="7bb0b-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="7bb0b-124">customErrorMessage</span></span>|<span data-ttu-id="7bb0b-125">String</span><span class="sxs-lookup"><span data-stu-id="7bb0b-125">String</span></span>|<span data-ttu-id="7bb0b-126">Задать пользовательское сообщение об ошибке для отображения после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="7bb0b-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="7bb0b-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="7bb0b-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="7bb0b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7bb0b-128">Int32</span></span>|<span data-ttu-id="7bb0b-129">Задать время ожидания ход выполнения установки в минутах</span><span class="sxs-lookup"><span data-stu-id="7bb0b-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="7bb0b-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="7bb0b-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="7bb0b-131">Логический</span><span class="sxs-lookup"><span data-stu-id="7bb0b-131">Boolean</span></span>|<span data-ttu-id="7bb0b-132">Разрешает пользователю продолжить использование устройства на сбой установки</span><span class="sxs-lookup"><span data-stu-id="7bb0b-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bb0b-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="7bb0b-133">Relationships</span></span>
<span data-ttu-id="7bb0b-134">Нет</span><span class="sxs-lookup"><span data-stu-id="7bb0b-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bb0b-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bb0b-135">JSON Representation</span></span>
<span data-ttu-id="7bb0b-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bb0b-136">Here is a JSON representation of the resource.</span></span>
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




