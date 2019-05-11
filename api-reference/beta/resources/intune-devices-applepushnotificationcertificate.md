---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9adcc496943118f268b8977a4134c4e434130bad
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943209"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="134f4-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="134f4-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="134f4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="134f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="134f4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="134f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="134f4-106">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="134f4-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="134f4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="134f4-107">Methods</span></span>
|<span data-ttu-id="134f4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="134f4-108">Method</span></span>|<span data-ttu-id="134f4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="134f4-109">Return Type</span></span>|<span data-ttu-id="134f4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="134f4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="134f4-111">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="134f4-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="134f4-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="134f4-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="134f4-113">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="134f4-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="134f4-114">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="134f4-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="134f4-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="134f4-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="134f4-116">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="134f4-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="134f4-117">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="134f4-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="134f4-118">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-118">String</span></span>|<span data-ttu-id="134f4-119">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="134f4-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="134f4-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="134f4-120">Properties</span></span>
|<span data-ttu-id="134f4-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="134f4-121">Property</span></span>|<span data-ttu-id="134f4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="134f4-122">Type</span></span>|<span data-ttu-id="134f4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="134f4-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="134f4-124">id</span><span class="sxs-lookup"><span data-stu-id="134f4-124">id</span></span>|<span data-ttu-id="134f4-125">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-125">String</span></span>|<span data-ttu-id="134f4-126">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="134f4-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="134f4-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="134f4-127">appleIdentifier</span></span>|<span data-ttu-id="134f4-128">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-128">String</span></span>|<span data-ttu-id="134f4-129">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="134f4-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="134f4-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="134f4-130">topicIdentifier</span></span>|<span data-ttu-id="134f4-131">String</span><span class="sxs-lookup"><span data-stu-id="134f4-131">String</span></span>|<span data-ttu-id="134f4-132">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="134f4-132">Topic Id.</span></span>|
|<span data-ttu-id="134f4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="134f4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="134f4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="134f4-134">DateTimeOffset</span></span>|<span data-ttu-id="134f4-135">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="134f4-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="134f4-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="134f4-136">expirationDateTime</span></span>|<span data-ttu-id="134f4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="134f4-137">DateTimeOffset</span></span>|<span data-ttu-id="134f4-138">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="134f4-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="134f4-139">Цертификатеуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="134f4-139">certificateUploadStatus</span></span>|<span data-ttu-id="134f4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-140">String</span></span>|<span data-ttu-id="134f4-141">Состояние отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="134f4-141">The certificate upload status.</span></span>|
|<span data-ttu-id="134f4-142">Цертификатеуплоадфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="134f4-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="134f4-143">Строка</span><span class="sxs-lookup"><span data-stu-id="134f4-143">String</span></span>|<span data-ttu-id="134f4-144">Причина сбоя отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="134f4-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="134f4-145">certificate</span><span class="sxs-lookup"><span data-stu-id="134f4-145">certificate</span></span>|<span data-ttu-id="134f4-146">String</span><span class="sxs-lookup"><span data-stu-id="134f4-146">String</span></span>|<span data-ttu-id="134f4-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="134f4-147">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="134f4-148">Связи</span><span class="sxs-lookup"><span data-stu-id="134f4-148">Relationships</span></span>
<span data-ttu-id="134f4-149">Нет</span><span class="sxs-lookup"><span data-stu-id="134f4-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="134f4-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="134f4-150">JSON Representation</span></span>
<span data-ttu-id="134f4-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="134f4-151">Here is a JSON representation of the resource.</span></span>
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




