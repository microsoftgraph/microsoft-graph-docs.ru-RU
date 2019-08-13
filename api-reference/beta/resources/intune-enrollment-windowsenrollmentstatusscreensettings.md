---
title: Тип ресурса Виндовсенроллментстатусскринсеттингс
description: Настройка экрана состояния регистрации
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f556b8e0f3bd634ce0e8bfe855d6615d9e58d623
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327670"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="bb401-103">Тип ресурса Виндовсенроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="bb401-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="bb401-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb401-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb401-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb401-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb401-106">Настройка экрана состояния регистрации</span><span class="sxs-lookup"><span data-stu-id="bb401-106">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="bb401-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb401-107">Properties</span></span>
|<span data-ttu-id="bb401-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb401-108">Property</span></span>|<span data-ttu-id="bb401-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bb401-109">Type</span></span>|<span data-ttu-id="bb401-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb401-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb401-111">хидеинсталлатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="bb401-111">hideInstallationProgress</span></span>|<span data-ttu-id="bb401-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb401-112">Boolean</span></span>|<span data-ttu-id="bb401-113">Отображение или скрытие хода установки для пользователя</span><span class="sxs-lookup"><span data-stu-id="bb401-113">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="bb401-114">алловдевицеусебефорепрофилеандаппинсталлкомплете</span><span class="sxs-lookup"><span data-stu-id="bb401-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="bb401-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb401-115">Boolean</span></span>|<span data-ttu-id="bb401-116">Разрешить или запретить пользователю использовать устройство до завершения установки профилей и приложений</span><span class="sxs-lookup"><span data-stu-id="bb401-116">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="bb401-117">блоккдевицесетупретрибюсер</span><span class="sxs-lookup"><span data-stu-id="bb401-117">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="bb401-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb401-118">Boolean</span></span>|<span data-ttu-id="bb401-119">Разрешить пользователю повторно выполнить установку при сбое установки</span><span class="sxs-lookup"><span data-stu-id="bb401-119">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="bb401-120">алловлогколлектиононинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="bb401-120">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="bb401-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb401-121">Boolean</span></span>|<span data-ttu-id="bb401-122">Разрешение или блокировка сбора журналов при сбое установки</span><span class="sxs-lookup"><span data-stu-id="bb401-122">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="bb401-123">кустомеррормессаже</span><span class="sxs-lookup"><span data-stu-id="bb401-123">customErrorMessage</span></span>|<span data-ttu-id="bb401-124">String</span><span class="sxs-lookup"><span data-stu-id="bb401-124">String</span></span>|<span data-ttu-id="bb401-125">Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки</span><span class="sxs-lookup"><span data-stu-id="bb401-125">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="bb401-126">инсталлпрогресстимеаутинминутес</span><span class="sxs-lookup"><span data-stu-id="bb401-126">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="bb401-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bb401-127">Int32</span></span>|<span data-ttu-id="bb401-128">Задать время ожидания установки (в минутах)</span><span class="sxs-lookup"><span data-stu-id="bb401-128">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="bb401-129">алловдевицеусеонинсталлфаилуре</span><span class="sxs-lookup"><span data-stu-id="bb401-129">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="bb401-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb401-130">Boolean</span></span>|<span data-ttu-id="bb401-131">Разрешить пользователю продолжать использовать устройство при сбое установки</span><span class="sxs-lookup"><span data-stu-id="bb401-131">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb401-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="bb401-132">Relationships</span></span>
<span data-ttu-id="bb401-133">Нет</span><span class="sxs-lookup"><span data-stu-id="bb401-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb401-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb401-134">JSON Representation</span></span>
<span data-ttu-id="bb401-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb401-135">Here is a JSON representation of the resource.</span></span>
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



