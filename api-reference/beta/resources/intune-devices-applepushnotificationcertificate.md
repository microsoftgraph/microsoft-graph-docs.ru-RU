---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eae13a9323a061de3bd5128bb55a80c4d4bc3b35
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983339"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="061bb-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="061bb-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="061bb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="061bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="061bb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="061bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="061bb-106">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="061bb-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="061bb-107">Методы</span><span class="sxs-lookup"><span data-stu-id="061bb-107">Methods</span></span>
|<span data-ttu-id="061bb-108">Метод</span><span class="sxs-lookup"><span data-stu-id="061bb-108">Method</span></span>|<span data-ttu-id="061bb-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="061bb-109">Return Type</span></span>|<span data-ttu-id="061bb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="061bb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="061bb-111">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="061bb-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="061bb-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="061bb-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="061bb-113">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="061bb-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="061bb-114">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="061bb-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="061bb-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="061bb-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="061bb-116">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="061bb-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="061bb-117">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="061bb-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="061bb-118">String</span><span class="sxs-lookup"><span data-stu-id="061bb-118">String</span></span>|<span data-ttu-id="061bb-119">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="061bb-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="061bb-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="061bb-120">Properties</span></span>
|<span data-ttu-id="061bb-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="061bb-121">Property</span></span>|<span data-ttu-id="061bb-122">Тип</span><span class="sxs-lookup"><span data-stu-id="061bb-122">Type</span></span>|<span data-ttu-id="061bb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="061bb-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="061bb-124">id</span><span class="sxs-lookup"><span data-stu-id="061bb-124">id</span></span>|<span data-ttu-id="061bb-125">String</span><span class="sxs-lookup"><span data-stu-id="061bb-125">String</span></span>|<span data-ttu-id="061bb-126">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="061bb-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="061bb-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="061bb-127">appleIdentifier</span></span>|<span data-ttu-id="061bb-128">String</span><span class="sxs-lookup"><span data-stu-id="061bb-128">String</span></span>|<span data-ttu-id="061bb-129">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="061bb-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="061bb-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="061bb-130">topicIdentifier</span></span>|<span data-ttu-id="061bb-131">String</span><span class="sxs-lookup"><span data-stu-id="061bb-131">String</span></span>|<span data-ttu-id="061bb-132">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="061bb-132">Topic Id.</span></span>|
|<span data-ttu-id="061bb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="061bb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="061bb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="061bb-134">DateTimeOffset</span></span>|<span data-ttu-id="061bb-135">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="061bb-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="061bb-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="061bb-136">expirationDateTime</span></span>|<span data-ttu-id="061bb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="061bb-137">DateTimeOffset</span></span>|<span data-ttu-id="061bb-138">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="061bb-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="061bb-139">Цертификатеуплоадстатус</span><span class="sxs-lookup"><span data-stu-id="061bb-139">certificateUploadStatus</span></span>|<span data-ttu-id="061bb-140">String</span><span class="sxs-lookup"><span data-stu-id="061bb-140">String</span></span>|<span data-ttu-id="061bb-141">Состояние отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="061bb-141">The certificate upload status.</span></span>|
|<span data-ttu-id="061bb-142">Цертификатеуплоадфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="061bb-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="061bb-143">String</span><span class="sxs-lookup"><span data-stu-id="061bb-143">String</span></span>|<span data-ttu-id="061bb-144">Причина сбоя отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="061bb-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="061bb-145">certificate</span><span class="sxs-lookup"><span data-stu-id="061bb-145">certificate</span></span>|<span data-ttu-id="061bb-146">String</span><span class="sxs-lookup"><span data-stu-id="061bb-146">String</span></span>|<span data-ttu-id="061bb-147">Н/Д</span><span class="sxs-lookup"><span data-stu-id="061bb-147">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="061bb-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="061bb-148">Relationships</span></span>
<span data-ttu-id="061bb-149">Нет</span><span class="sxs-lookup"><span data-stu-id="061bb-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="061bb-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="061bb-150">JSON Representation</span></span>
<span data-ttu-id="061bb-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="061bb-151">Here is a JSON representation of the resource.</span></span>
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





