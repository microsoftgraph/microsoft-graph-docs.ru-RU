---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79c7bcd1bfe7a1eac1820cbe7163cac0b2b5311e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451318"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="5da8b-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5da8b-103">applePushNotificationCertificate resource type</span></span>

<span data-ttu-id="5da8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5da8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5da8b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5da8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5da8b-106">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="5da8b-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="5da8b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5da8b-107">Methods</span></span>
|<span data-ttu-id="5da8b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5da8b-108">Method</span></span>|<span data-ttu-id="5da8b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5da8b-109">Return Type</span></span>|<span data-ttu-id="5da8b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5da8b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5da8b-111">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5da8b-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="5da8b-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5da8b-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="5da8b-113">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5da8b-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="5da8b-114">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5da8b-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="5da8b-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5da8b-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="5da8b-116">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="5da8b-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="5da8b-117">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="5da8b-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="5da8b-118">String</span><span class="sxs-lookup"><span data-stu-id="5da8b-118">String</span></span>|<span data-ttu-id="5da8b-119">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="5da8b-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="5da8b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="5da8b-120">Properties</span></span>
|<span data-ttu-id="5da8b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="5da8b-121">Property</span></span>|<span data-ttu-id="5da8b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5da8b-122">Type</span></span>|<span data-ttu-id="5da8b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5da8b-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5da8b-124">id</span><span class="sxs-lookup"><span data-stu-id="5da8b-124">id</span></span>|<span data-ttu-id="5da8b-125">String</span><span class="sxs-lookup"><span data-stu-id="5da8b-125">String</span></span>|<span data-ttu-id="5da8b-126">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="5da8b-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="5da8b-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="5da8b-127">appleIdentifier</span></span>|<span data-ttu-id="5da8b-128">String</span><span class="sxs-lookup"><span data-stu-id="5da8b-128">String</span></span>|<span data-ttu-id="5da8b-129">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="5da8b-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="5da8b-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="5da8b-130">topicIdentifier</span></span>|<span data-ttu-id="5da8b-131">String</span><span class="sxs-lookup"><span data-stu-id="5da8b-131">String</span></span>|<span data-ttu-id="5da8b-132">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="5da8b-132">Topic Id.</span></span>|
|<span data-ttu-id="5da8b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5da8b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5da8b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5da8b-134">DateTimeOffset</span></span>|<span data-ttu-id="5da8b-135">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="5da8b-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5da8b-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5da8b-136">expirationDateTime</span></span>|<span data-ttu-id="5da8b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5da8b-137">DateTimeOffset</span></span>|<span data-ttu-id="5da8b-138">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="5da8b-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="5da8b-139">certificate</span><span class="sxs-lookup"><span data-stu-id="5da8b-139">certificate</span></span>|<span data-ttu-id="5da8b-140">String</span><span class="sxs-lookup"><span data-stu-id="5da8b-140">String</span></span>|<span data-ttu-id="5da8b-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5da8b-141">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="5da8b-142">Связи</span><span class="sxs-lookup"><span data-stu-id="5da8b-142">Relationships</span></span>
<span data-ttu-id="5da8b-143">Нет</span><span class="sxs-lookup"><span data-stu-id="5da8b-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5da8b-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5da8b-144">JSON Representation</span></span>
<span data-ttu-id="5da8b-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5da8b-145">Here is a JSON representation of the resource.</span></span>
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







