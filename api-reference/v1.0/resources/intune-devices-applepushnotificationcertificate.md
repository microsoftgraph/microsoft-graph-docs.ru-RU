---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f07561029d35d945eca118f095496891c73a25a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941739"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="d5afc-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d5afc-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="d5afc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d5afc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5afc-105">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="d5afc-105">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="d5afc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d5afc-106">Methods</span></span>
|<span data-ttu-id="d5afc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d5afc-107">Method</span></span>|<span data-ttu-id="d5afc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d5afc-108">Return Type</span></span>|<span data-ttu-id="d5afc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d5afc-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5afc-110">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d5afc-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="d5afc-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d5afc-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="d5afc-112">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d5afc-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="d5afc-113">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d5afc-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="d5afc-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d5afc-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="d5afc-115">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d5afc-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="d5afc-116">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="d5afc-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="d5afc-117">String</span><span class="sxs-lookup"><span data-stu-id="d5afc-117">String</span></span>|<span data-ttu-id="d5afc-118">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="d5afc-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="d5afc-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5afc-119">Properties</span></span>
|<span data-ttu-id="d5afc-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5afc-120">Property</span></span>|<span data-ttu-id="d5afc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d5afc-121">Type</span></span>|<span data-ttu-id="d5afc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d5afc-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5afc-123">id</span><span class="sxs-lookup"><span data-stu-id="d5afc-123">id</span></span>|<span data-ttu-id="d5afc-124">String</span><span class="sxs-lookup"><span data-stu-id="d5afc-124">String</span></span>|<span data-ttu-id="d5afc-125">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="d5afc-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="d5afc-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5afc-126">appleIdentifier</span></span>|<span data-ttu-id="d5afc-127">String</span><span class="sxs-lookup"><span data-stu-id="d5afc-127">String</span></span>|<span data-ttu-id="d5afc-128">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="d5afc-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="d5afc-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="d5afc-129">topicIdentifier</span></span>|<span data-ttu-id="d5afc-130">String</span><span class="sxs-lookup"><span data-stu-id="d5afc-130">String</span></span>|<span data-ttu-id="d5afc-131">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="d5afc-131">Topic Id.</span></span>|
|<span data-ttu-id="d5afc-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5afc-132">lastModifiedDateTime</span></span>|<span data-ttu-id="d5afc-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5afc-133">DateTimeOffset</span></span>|<span data-ttu-id="d5afc-134">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="d5afc-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d5afc-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d5afc-135">expirationDateTime</span></span>|<span data-ttu-id="d5afc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5afc-136">DateTimeOffset</span></span>|<span data-ttu-id="d5afc-137">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="d5afc-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d5afc-138">certificate</span><span class="sxs-lookup"><span data-stu-id="d5afc-138">certificate</span></span>|<span data-ttu-id="d5afc-139">String</span><span class="sxs-lookup"><span data-stu-id="d5afc-139">String</span></span>|<span data-ttu-id="d5afc-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d5afc-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5afc-141">Связи</span><span class="sxs-lookup"><span data-stu-id="d5afc-141">Relationships</span></span>
<span data-ttu-id="d5afc-142">Нет</span><span class="sxs-lookup"><span data-stu-id="d5afc-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5afc-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5afc-143">JSON Representation</span></span>
<span data-ttu-id="d5afc-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5afc-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



