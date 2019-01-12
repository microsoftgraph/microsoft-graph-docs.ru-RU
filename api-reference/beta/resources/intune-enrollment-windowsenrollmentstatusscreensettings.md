---
title: Тип ресурса windowsEnrollmentStatusScreenSettings
description: Параметр экрана состояния подачи заявок
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: abc48a1d63cc514d2ec887a7758e69a0ea8112a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978573"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="b5c0a-103">Тип ресурса windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="b5c0a-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="b5c0a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b5c0a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5c0a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5c0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5c0a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b5c0a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5c0a-107">Параметр экрана состояния подачи заявок</span><span class="sxs-lookup"><span data-stu-id="b5c0a-107">Enrollment status screen setting</span></span>
## <a name="properties"></a><span data-ttu-id="b5c0a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5c0a-108">Properties</span></span>
|<span data-ttu-id="b5c0a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5c0a-109">Property</span></span>|<span data-ttu-id="b5c0a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b5c0a-110">Type</span></span>|<span data-ttu-id="b5c0a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b5c0a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5c0a-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="b5c0a-112">hideInstallationProgress</span></span>|<span data-ttu-id="b5c0a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5c0a-113">Boolean</span></span>|<span data-ttu-id="b5c0a-114">Показать или скрыть выполнения установки для пользователей</span><span class="sxs-lookup"><span data-stu-id="b5c0a-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="b5c0a-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="b5c0a-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="b5c0a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5c0a-116">Boolean</span></span>|<span data-ttu-id="b5c0a-117">Разрешить или заблокировать пользователя для использования устройств до завершения установки приложения и профилей</span><span class="sxs-lookup"><span data-stu-id="b5c0a-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="b5c0a-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="b5c0a-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="b5c0a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5c0a-119">Boolean</span></span>|<span data-ttu-id="b5c0a-120">Пользователь может повторно запустите программу установки на сбой установки</span><span class="sxs-lookup"><span data-stu-id="b5c0a-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="b5c0a-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b5c0a-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="b5c0a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5c0a-122">Boolean</span></span>|<span data-ttu-id="b5c0a-123">Разрешить или заблокировать семейства журнала на сбой установки</span><span class="sxs-lookup"><span data-stu-id="b5c0a-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="b5c0a-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="b5c0a-124">customErrorMessage</span></span>|<span data-ttu-id="b5c0a-125">String</span><span class="sxs-lookup"><span data-stu-id="b5c0a-125">String</span></span>|<span data-ttu-id="b5c0a-126">Задать пользовательское сообщение об ошибке для отображения после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="b5c0a-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="b5c0a-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b5c0a-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="b5c0a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b5c0a-128">Int32</span></span>|<span data-ttu-id="b5c0a-129">Задать время ожидания ход выполнения установки в минутах</span><span class="sxs-lookup"><span data-stu-id="b5c0a-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="b5c0a-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b5c0a-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="b5c0a-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5c0a-131">Boolean</span></span>|<span data-ttu-id="b5c0a-132">Разрешает пользователю продолжить использование устройства на сбой установки</span><span class="sxs-lookup"><span data-stu-id="b5c0a-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5c0a-133">Связи</span><span class="sxs-lookup"><span data-stu-id="b5c0a-133">Relationships</span></span>
<span data-ttu-id="b5c0a-134">Нет</span><span class="sxs-lookup"><span data-stu-id="b5c0a-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5c0a-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5c0a-135">JSON Representation</span></span>
<span data-ttu-id="b5c0a-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5c0a-136">Here is a JSON representation of the resource.</span></span>
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





