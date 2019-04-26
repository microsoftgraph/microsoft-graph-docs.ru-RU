---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41d5161f1e9344f187329bf795219151c91f29ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555887"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="881aa-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="881aa-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="881aa-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="881aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="881aa-105">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="881aa-105">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="881aa-106">Методы</span><span class="sxs-lookup"><span data-stu-id="881aa-106">Methods</span></span>
|<span data-ttu-id="881aa-107">Метод</span><span class="sxs-lookup"><span data-stu-id="881aa-107">Method</span></span>|<span data-ttu-id="881aa-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="881aa-108">Return Type</span></span>|<span data-ttu-id="881aa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="881aa-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="881aa-110">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="881aa-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="881aa-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="881aa-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="881aa-112">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="881aa-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="881aa-113">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="881aa-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="881aa-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="881aa-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="881aa-115">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="881aa-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="881aa-116">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="881aa-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="881aa-117">String</span><span class="sxs-lookup"><span data-stu-id="881aa-117">String</span></span>|<span data-ttu-id="881aa-118">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="881aa-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="881aa-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="881aa-119">Properties</span></span>
|<span data-ttu-id="881aa-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="881aa-120">Property</span></span>|<span data-ttu-id="881aa-121">Тип</span><span class="sxs-lookup"><span data-stu-id="881aa-121">Type</span></span>|<span data-ttu-id="881aa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="881aa-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="881aa-123">id</span><span class="sxs-lookup"><span data-stu-id="881aa-123">id</span></span>|<span data-ttu-id="881aa-124">String</span><span class="sxs-lookup"><span data-stu-id="881aa-124">String</span></span>|<span data-ttu-id="881aa-125">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="881aa-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="881aa-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="881aa-126">appleIdentifier</span></span>|<span data-ttu-id="881aa-127">String</span><span class="sxs-lookup"><span data-stu-id="881aa-127">String</span></span>|<span data-ttu-id="881aa-128">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="881aa-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="881aa-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="881aa-129">topicIdentifier</span></span>|<span data-ttu-id="881aa-130">String</span><span class="sxs-lookup"><span data-stu-id="881aa-130">String</span></span>|<span data-ttu-id="881aa-131">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="881aa-131">Topic Id.</span></span>|
|<span data-ttu-id="881aa-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="881aa-132">lastModifiedDateTime</span></span>|<span data-ttu-id="881aa-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="881aa-133">DateTimeOffset</span></span>|<span data-ttu-id="881aa-134">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="881aa-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="881aa-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="881aa-135">expirationDateTime</span></span>|<span data-ttu-id="881aa-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="881aa-136">DateTimeOffset</span></span>|<span data-ttu-id="881aa-137">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="881aa-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="881aa-138">certificate</span><span class="sxs-lookup"><span data-stu-id="881aa-138">certificate</span></span>|<span data-ttu-id="881aa-139">String</span><span class="sxs-lookup"><span data-stu-id="881aa-139">String</span></span>|<span data-ttu-id="881aa-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="881aa-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="881aa-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="881aa-141">Relationships</span></span>
<span data-ttu-id="881aa-142">Нет</span><span class="sxs-lookup"><span data-stu-id="881aa-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="881aa-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="881aa-143">JSON Representation</span></span>
<span data-ttu-id="881aa-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="881aa-144">Here is a JSON representation of the resource.</span></span>
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



