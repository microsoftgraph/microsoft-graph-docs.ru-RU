---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d4a5725c6cd046c4baa34316f74a90b4c9fb05f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000048"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="1a265-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="1a265-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="1a265-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a265-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a265-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a265-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a265-106">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="1a265-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="1a265-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1a265-107">Methods</span></span>
|<span data-ttu-id="1a265-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1a265-108">Method</span></span>|<span data-ttu-id="1a265-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1a265-109">Return Type</span></span>|<span data-ttu-id="1a265-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a265-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a265-111">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="1a265-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="1a265-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="1a265-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="1a265-113">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="1a265-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="1a265-114">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="1a265-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="1a265-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="1a265-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="1a265-116">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="1a265-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="1a265-117">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="1a265-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="1a265-118">String</span><span class="sxs-lookup"><span data-stu-id="1a265-118">String</span></span>|<span data-ttu-id="1a265-119">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="1a265-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="1a265-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a265-120">Properties</span></span>
|<span data-ttu-id="1a265-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a265-121">Property</span></span>|<span data-ttu-id="1a265-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1a265-122">Type</span></span>|<span data-ttu-id="1a265-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1a265-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a265-124">id</span><span class="sxs-lookup"><span data-stu-id="1a265-124">id</span></span>|<span data-ttu-id="1a265-125">String</span><span class="sxs-lookup"><span data-stu-id="1a265-125">String</span></span>|<span data-ttu-id="1a265-126">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="1a265-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="1a265-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a265-127">appleIdentifier</span></span>|<span data-ttu-id="1a265-128">String</span><span class="sxs-lookup"><span data-stu-id="1a265-128">String</span></span>|<span data-ttu-id="1a265-129">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="1a265-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="1a265-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a265-130">topicIdentifier</span></span>|<span data-ttu-id="1a265-131">String</span><span class="sxs-lookup"><span data-stu-id="1a265-131">String</span></span>|<span data-ttu-id="1a265-132">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="1a265-132">Topic Id.</span></span>|
|<span data-ttu-id="1a265-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a265-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1a265-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a265-134">DateTimeOffset</span></span>|<span data-ttu-id="1a265-135">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="1a265-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1a265-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a265-136">expirationDateTime</span></span>|<span data-ttu-id="1a265-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a265-137">DateTimeOffset</span></span>|<span data-ttu-id="1a265-138">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="1a265-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="1a265-139">Цертификатеуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="1a265-139">certificateUploadStatus</span></span>|<span data-ttu-id="1a265-140">String</span><span class="sxs-lookup"><span data-stu-id="1a265-140">String</span></span>|<span data-ttu-id="1a265-141">Состояние отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="1a265-141">The certificate upload status.</span></span>|
|<span data-ttu-id="1a265-142">Цертификатеуплоадфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="1a265-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="1a265-143">String</span><span class="sxs-lookup"><span data-stu-id="1a265-143">String</span></span>|<span data-ttu-id="1a265-144">Причина сбоя отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="1a265-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="1a265-145">certificate</span><span class="sxs-lookup"><span data-stu-id="1a265-145">certificate</span></span>|<span data-ttu-id="1a265-146">String</span><span class="sxs-lookup"><span data-stu-id="1a265-146">String</span></span>|<span data-ttu-id="1a265-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1a265-147">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a265-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="1a265-148">Relationships</span></span>
<span data-ttu-id="1a265-149">Нет</span><span class="sxs-lookup"><span data-stu-id="1a265-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a265-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a265-150">JSON Representation</span></span>
<span data-ttu-id="1a265-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a265-151">Here is a JSON representation of the resource.</span></span>
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
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificate": "String"
}
```





