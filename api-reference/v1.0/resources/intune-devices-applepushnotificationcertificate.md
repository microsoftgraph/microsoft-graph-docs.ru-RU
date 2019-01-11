---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 43a697feaab14589540747ff0f4f79ca194918ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856845"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="e914d-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e914d-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="e914d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e914d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e914d-105">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="e914d-105">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="e914d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e914d-106">Methods</span></span>
|<span data-ttu-id="e914d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e914d-107">Method</span></span>|<span data-ttu-id="e914d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e914d-108">Return Type</span></span>|<span data-ttu-id="e914d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e914d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e914d-110">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e914d-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="e914d-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e914d-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="e914d-112">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e914d-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="e914d-113">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e914d-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="e914d-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e914d-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="e914d-115">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e914d-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="e914d-116">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="e914d-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="e914d-117">String</span><span class="sxs-lookup"><span data-stu-id="e914d-117">String</span></span>|<span data-ttu-id="e914d-118">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="e914d-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="e914d-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e914d-119">Properties</span></span>
|<span data-ttu-id="e914d-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e914d-120">Property</span></span>|<span data-ttu-id="e914d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e914d-121">Type</span></span>|<span data-ttu-id="e914d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e914d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e914d-123">id</span><span class="sxs-lookup"><span data-stu-id="e914d-123">id</span></span>|<span data-ttu-id="e914d-124">String</span><span class="sxs-lookup"><span data-stu-id="e914d-124">String</span></span>|<span data-ttu-id="e914d-125">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="e914d-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="e914d-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="e914d-126">appleIdentifier</span></span>|<span data-ttu-id="e914d-127">String</span><span class="sxs-lookup"><span data-stu-id="e914d-127">String</span></span>|<span data-ttu-id="e914d-128">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="e914d-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="e914d-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="e914d-129">topicIdentifier</span></span>|<span data-ttu-id="e914d-130">String</span><span class="sxs-lookup"><span data-stu-id="e914d-130">String</span></span>|<span data-ttu-id="e914d-131">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="e914d-131">Topic Id.</span></span>|
|<span data-ttu-id="e914d-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e914d-132">lastModifiedDateTime</span></span>|<span data-ttu-id="e914d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e914d-133">DateTimeOffset</span></span>|<span data-ttu-id="e914d-134">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="e914d-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="e914d-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e914d-135">expirationDateTime</span></span>|<span data-ttu-id="e914d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e914d-136">DateTimeOffset</span></span>|<span data-ttu-id="e914d-137">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="e914d-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="e914d-138">certificate</span><span class="sxs-lookup"><span data-stu-id="e914d-138">certificate</span></span>|<span data-ttu-id="e914d-139">String</span><span class="sxs-lookup"><span data-stu-id="e914d-139">String</span></span>|<span data-ttu-id="e914d-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e914d-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="e914d-141">Связи</span><span class="sxs-lookup"><span data-stu-id="e914d-141">Relationships</span></span>
<span data-ttu-id="e914d-142">Нет</span><span class="sxs-lookup"><span data-stu-id="e914d-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e914d-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e914d-143">JSON Representation</span></span>
<span data-ttu-id="e914d-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e914d-144">Here is a JSON representation of the resource.</span></span>
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



