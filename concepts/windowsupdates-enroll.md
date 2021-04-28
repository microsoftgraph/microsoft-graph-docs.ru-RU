---
title: Регистрация в управлении обновлениями службой Windows обновления для бизнеса
description: Когда устройство зачислилось в управление обновлениями службой развертывания Windows для бизнеса, вы можете использовать службу развертывания для управления контентом, доставленным из Windows Update на это устройство.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 2492a447aa26bbc3de6835a76c5876e55cac774c
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067742"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a><span data-ttu-id="a7aee-103">Регистрация в управлении обновлениями службой Windows обновления для бизнеса</span><span class="sxs-lookup"><span data-stu-id="a7aee-103">Enroll in update management by the Windows Update for Business deployment service</span></span>

<span data-ttu-id="a7aee-104">При регистрации устройства в управлении обновлениями службой развертывания Windows обновления для бизнеса можно использовать службу развертывания для управления контентом, доставленным из Windows Update на это устройство.</span><span class="sxs-lookup"><span data-stu-id="a7aee-104">When you enroll device in update management by the Windows Update for Business deployment service, you can use the deployment service to manage content delivered from Windows Update to that device.</span></span> <span data-ttu-id="a7aee-105">Вы можете записать устройство в управление обновлениями по категории обновления.</span><span class="sxs-lookup"><span data-stu-id="a7aee-105">You can enroll a device in update management by update category.</span></span>

<span data-ttu-id="a7aee-106">Сегодня служба развертывания поддерживает регистрацию в управлении обновлениями Windows 10 функций.</span><span class="sxs-lookup"><span data-stu-id="a7aee-106">Today, the deployment service supports enrollment in management of Windows 10 feature updates.</span></span> <span data-ttu-id="a7aee-107">В настоящее время служба развертывания не требует регистрации в управлении обновлениями Windows 10 качества, чтобы развернуть ускоренные обновления качества.</span><span class="sxs-lookup"><span data-stu-id="a7aee-107">At this time, the deployment service does not require enrollment in management of Windows 10 quality updates in order to deploy expedited quality updates.</span></span>

## <a name="enroll-the-device-in-update-management"></a><span data-ttu-id="a7aee-108">Регистрация устройства в управлении обновлениями</span><span class="sxs-lookup"><span data-stu-id="a7aee-108">Enroll the device in update management</span></span>

<span data-ttu-id="a7aee-109">При регистрации устройства в управлении для определенной категории обновлений служба развертывания становится органом для обновлений этой категории, исходя из Windows Update.</span><span class="sxs-lookup"><span data-stu-id="a7aee-109">When you enroll a device in management for a certain update category, the deployment service becomes the authority for updates of that category coming from Windows Update.</span></span> <span data-ttu-id="a7aee-110">В результате устройства не получают обновления этой категории из Windows, пока не развернуто обновление с помощью службы развертывания, назначив его [развертыванию.](windowsupdates-deployments.md)</span><span class="sxs-lookup"><span data-stu-id="a7aee-110">As a result, devices do not receive updates of that category from Windows Update until you deploy an update using the deployment service by assigning it to a [deployment](windowsupdates-deployments.md).</span></span> <span data-ttu-id="a7aee-111">Устройства автоматически регистрируются в службе при регистрации в управлении службой (например, объект [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice.md) автоматически создается, если он еще не существует).</span><span class="sxs-lookup"><span data-stu-id="a7aee-111">Devices are automatically registered with the service when enrolled in management by the service (i.e. an [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice.md) object is automatically created if it does not already exist).</span></span>

### <a name="request"></a><span data-ttu-id="a7aee-112">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7aee-112">Request</span></span>

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a7aee-113">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7aee-113">Response</span></span>

``` http
HTTP/1.1 202 Accepted
```

## <a name="check-the-enrollment-state-of-a-device"></a><span data-ttu-id="a7aee-114">Проверка состояния регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="a7aee-114">Check the enrollment state of a device</span></span>

<span data-ttu-id="a7aee-115">Вы можете проверить состояние регистрации [](/graph/api/windowsupdates-azureaddevice-get) устройства, получив устройство  и посмотрев свойства регистраций и ошибок на **объекте azureADDevice.** </span><span class="sxs-lookup"><span data-stu-id="a7aee-115">You can check the enrollment state of a device by [getting the device](/graph/api/windowsupdates-azureaddevice-get) and looking at the **enrollments** and **errors** properties on the **azureADDevice** object.</span></span> <span data-ttu-id="a7aee-116">Устройство, успешно зарегистрированное в управлении обновлениями, имеет объект [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) в коллекции регистраций и не имеет объектов [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) в коллекции ошибок.</span><span class="sxs-lookup"><span data-stu-id="a7aee-116">A device that is successfully enrolled in update management has an [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) object in the enrollments collection, and it does not have any [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) objects in the errors collection.</span></span> <span data-ttu-id="a7aee-117">Устройство, которое служба пыталась зарегистрировать, но столкнулось с ошибкой, заполнялось коллекциями как для регистрации, так и для ошибок.</span><span class="sxs-lookup"><span data-stu-id="a7aee-117">A device that the service tried to enroll but encountered an error has populated collections for both enrollments and errors.</span></span> <span data-ttu-id="a7aee-118">Устройство, для которого служба не получала запросов на регистрацию, имеет пустые коллекции как для регистрации, так и для ошибок.</span><span class="sxs-lookup"><span data-stu-id="a7aee-118">A device for which the service has not received any enrollment requests has empty collections for both enrollments and errors.</span></span>

<span data-ttu-id="a7aee-119">В следующем примере показано устройство, успешно зарегистрированное службой в управлении обновлениями функций.</span><span class="sxs-lookup"><span data-stu-id="a7aee-119">The following example shows a device that is successfully enrolled in management of feature updates by the service.</span></span>

### <a name="request"></a><span data-ttu-id="a7aee-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7aee-120">Request</span></span>

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```

### <a name="response"></a><span data-ttu-id="a7aee-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7aee-121">Response</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a><span data-ttu-id="a7aee-122">Отстранить от управления службой или оторегистрить из службы</span><span class="sxs-lookup"><span data-stu-id="a7aee-122">Unenroll from management by the service or unregister from the service</span></span> 

<span data-ttu-id="a7aee-123">При откреплении устройства от управления службой для данной категории обновлений устройство больше не управляется службой развертывания и может начать получать другие обновления из Windows Update в зависимости от конфигурации политики.</span><span class="sxs-lookup"><span data-stu-id="a7aee-123">When you unenroll a device from management by the service for a given update category, the device is no longer managed by the deployment service and may start receiving other updates from Windows Update based on its policy configuration.</span></span> <span data-ttu-id="a7aee-124">Если устройство назначено любому развертыванию для данной категории обновлений, оно не получает этого контента.</span><span class="sxs-lookup"><span data-stu-id="a7aee-124">If the device is assigned to any deployments for the given update category, it does not receive that content.</span></span> <span data-ttu-id="a7aee-125">Устройство остается зарегистрированным в службе и по-прежнему регистрируется и получает контент для других категорий обновлений (если это применимо).</span><span class="sxs-lookup"><span data-stu-id="a7aee-125">The device remains registered with the service and is still enrolled and receiving content for other update categories (if applicable).</span></span>

### <a name="request"></a><span data-ttu-id="a7aee-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7aee-126">Request</span></span>

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a7aee-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7aee-127">Response</span></span>

``` http
HTTP/1.1 202 Accepted
```

<span data-ttu-id="a7aee-128">Вы можете полностью оторегистрить устройство из службы, удалив объект устройства.</span><span class="sxs-lookup"><span data-stu-id="a7aee-128">You can unregister a device from the service completely by deleting the device object.</span></span> <span data-ttu-id="a7aee-129">При незарегистрированной регистрации устройство автоматически отключается от управления службой для всех категорий обновлений и удаляется из всех аудиторий развертывания и [updatableAsset](/graph/api/resources/windowsupdates-updatableasset) групп.</span><span class="sxs-lookup"><span data-stu-id="a7aee-129">When a device is unregistered, it is automatically unenrolled from management by the service for all update categories and removed from all deployment audiences and [updatableAsset](/graph/api/resources/windowsupdates-updatableasset) groups.</span></span>

### <a name="request"></a><span data-ttu-id="a7aee-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7aee-130">Request</span></span>

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a><span data-ttu-id="a7aee-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7aee-131">Response</span></span>
``` http
HTTP/1.1 202 Accepted
```

