---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8a5df851f1826cd3e1e124bf8c2cda89b24da8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395589"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="935cb-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="935cb-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="935cb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="935cb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="935cb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="935cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="935cb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="935cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="935cb-107">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="935cb-107">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="935cb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="935cb-108">Methods</span></span>
|<span data-ttu-id="935cb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="935cb-109">Method</span></span>|<span data-ttu-id="935cb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="935cb-110">Return Type</span></span>|<span data-ttu-id="935cb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="935cb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="935cb-112">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="935cb-112">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="935cb-113">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="935cb-113">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="935cb-114">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="935cb-114">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="935cb-115">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="935cb-115">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="935cb-116">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="935cb-116">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="935cb-117">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="935cb-117">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="935cb-118">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="935cb-118">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="935cb-119">String</span><span class="sxs-lookup"><span data-stu-id="935cb-119">String</span></span>|<span data-ttu-id="935cb-120">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="935cb-120">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="935cb-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="935cb-121">Properties</span></span>
|<span data-ttu-id="935cb-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="935cb-122">Property</span></span>|<span data-ttu-id="935cb-123">Тип</span><span class="sxs-lookup"><span data-stu-id="935cb-123">Type</span></span>|<span data-ttu-id="935cb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="935cb-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="935cb-125">id</span><span class="sxs-lookup"><span data-stu-id="935cb-125">id</span></span>|<span data-ttu-id="935cb-126">String</span><span class="sxs-lookup"><span data-stu-id="935cb-126">String</span></span>|<span data-ttu-id="935cb-127">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="935cb-127">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="935cb-128">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="935cb-128">appleIdentifier</span></span>|<span data-ttu-id="935cb-129">String</span><span class="sxs-lookup"><span data-stu-id="935cb-129">String</span></span>|<span data-ttu-id="935cb-130">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="935cb-130">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="935cb-131">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="935cb-131">topicIdentifier</span></span>|<span data-ttu-id="935cb-132">String</span><span class="sxs-lookup"><span data-stu-id="935cb-132">String</span></span>|<span data-ttu-id="935cb-133">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="935cb-133">Topic Id.</span></span>|
|<span data-ttu-id="935cb-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="935cb-134">lastModifiedDateTime</span></span>|<span data-ttu-id="935cb-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="935cb-135">DateTimeOffset</span></span>|<span data-ttu-id="935cb-136">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="935cb-136">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="935cb-137">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="935cb-137">expirationDateTime</span></span>|<span data-ttu-id="935cb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="935cb-138">DateTimeOffset</span></span>|<span data-ttu-id="935cb-139">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="935cb-139">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="935cb-140">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="935cb-140">certificateUploadStatus</span></span>|<span data-ttu-id="935cb-141">String</span><span class="sxs-lookup"><span data-stu-id="935cb-141">String</span></span>|<span data-ttu-id="935cb-142">Состояние загрузки сертификата.</span><span class="sxs-lookup"><span data-stu-id="935cb-142">The certificate upload status.</span></span>|
|<span data-ttu-id="935cb-143">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="935cb-143">certificateUploadFailureReason</span></span>|<span data-ttu-id="935cb-144">String</span><span class="sxs-lookup"><span data-stu-id="935cb-144">String</span></span>|<span data-ttu-id="935cb-145">Не удалось причине отправки сертификата.</span><span class="sxs-lookup"><span data-stu-id="935cb-145">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="935cb-146">certificate</span><span class="sxs-lookup"><span data-stu-id="935cb-146">certificate</span></span>|<span data-ttu-id="935cb-147">String</span><span class="sxs-lookup"><span data-stu-id="935cb-147">String</span></span>|<span data-ttu-id="935cb-148">Н/Д</span><span class="sxs-lookup"><span data-stu-id="935cb-148">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="935cb-149">Связи</span><span class="sxs-lookup"><span data-stu-id="935cb-149">Relationships</span></span>
<span data-ttu-id="935cb-150">Нет</span><span class="sxs-lookup"><span data-stu-id="935cb-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="935cb-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="935cb-151">JSON Representation</span></span>
<span data-ttu-id="935cb-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="935cb-152">Here is a JSON representation of the resource.</span></span>
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




