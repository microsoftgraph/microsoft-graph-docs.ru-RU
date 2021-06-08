---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d53407d5ec380e7bfe11d50f6871eb6bbfb87aa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760211"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="81b11-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="81b11-103">applePushNotificationCertificate resource type</span></span>

<span data-ttu-id="81b11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81b11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81b11-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81b11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81b11-106">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="81b11-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="81b11-107">Методы</span><span class="sxs-lookup"><span data-stu-id="81b11-107">Methods</span></span>
|<span data-ttu-id="81b11-108">Метод</span><span class="sxs-lookup"><span data-stu-id="81b11-108">Method</span></span>|<span data-ttu-id="81b11-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81b11-109">Return Type</span></span>|<span data-ttu-id="81b11-110">Описание</span><span class="sxs-lookup"><span data-stu-id="81b11-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81b11-111">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="81b11-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="81b11-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="81b11-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="81b11-113">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="81b11-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="81b11-114">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="81b11-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="81b11-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="81b11-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="81b11-116">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="81b11-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="81b11-117">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="81b11-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="81b11-118">String</span><span class="sxs-lookup"><span data-stu-id="81b11-118">String</span></span>|<span data-ttu-id="81b11-119">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="81b11-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="81b11-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="81b11-120">Properties</span></span>
|<span data-ttu-id="81b11-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="81b11-121">Property</span></span>|<span data-ttu-id="81b11-122">Тип</span><span class="sxs-lookup"><span data-stu-id="81b11-122">Type</span></span>|<span data-ttu-id="81b11-123">Описание</span><span class="sxs-lookup"><span data-stu-id="81b11-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b11-124">id</span><span class="sxs-lookup"><span data-stu-id="81b11-124">id</span></span>|<span data-ttu-id="81b11-125">String</span><span class="sxs-lookup"><span data-stu-id="81b11-125">String</span></span>|<span data-ttu-id="81b11-126">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="81b11-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="81b11-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="81b11-127">appleIdentifier</span></span>|<span data-ttu-id="81b11-128">String</span><span class="sxs-lookup"><span data-stu-id="81b11-128">String</span></span>|<span data-ttu-id="81b11-129">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="81b11-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="81b11-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="81b11-130">topicIdentifier</span></span>|<span data-ttu-id="81b11-131">String</span><span class="sxs-lookup"><span data-stu-id="81b11-131">String</span></span>|<span data-ttu-id="81b11-132">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="81b11-132">Topic Id.</span></span>|
|<span data-ttu-id="81b11-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81b11-133">lastModifiedDateTime</span></span>|<span data-ttu-id="81b11-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81b11-134">DateTimeOffset</span></span>|<span data-ttu-id="81b11-135">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="81b11-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="81b11-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="81b11-136">expirationDateTime</span></span>|<span data-ttu-id="81b11-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81b11-137">DateTimeOffset</span></span>|<span data-ttu-id="81b11-138">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="81b11-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="81b11-139">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="81b11-139">certificateSerialNumber</span></span>|<span data-ttu-id="81b11-140">String</span><span class="sxs-lookup"><span data-stu-id="81b11-140">String</span></span>|<span data-ttu-id="81b11-141">Серийный номер сертификата.</span><span class="sxs-lookup"><span data-stu-id="81b11-141">Certificate serial number.</span></span> <span data-ttu-id="81b11-142">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81b11-142">This property is read-only.</span></span>|
|<span data-ttu-id="81b11-143">certificate</span><span class="sxs-lookup"><span data-stu-id="81b11-143">certificate</span></span>|<span data-ttu-id="81b11-144">String</span><span class="sxs-lookup"><span data-stu-id="81b11-144">String</span></span>|<span data-ttu-id="81b11-145">Н/Д</span><span class="sxs-lookup"><span data-stu-id="81b11-145">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="81b11-146">Связи</span><span class="sxs-lookup"><span data-stu-id="81b11-146">Relationships</span></span>
<span data-ttu-id="81b11-147">Нет</span><span class="sxs-lookup"><span data-stu-id="81b11-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81b11-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81b11-148">JSON Representation</span></span>
<span data-ttu-id="81b11-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81b11-149">Here is a JSON representation of the resource.</span></span>
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
  "certificateSerialNumber": "String",
  "certificate": "String"
}
```




