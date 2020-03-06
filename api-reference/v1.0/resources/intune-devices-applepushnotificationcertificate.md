---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 220bfa75c896693e5c7ff841a5f5957aab9decf0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530315"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="d57d4-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d57d4-103">applePushNotificationCertificate resource type</span></span>

<span data-ttu-id="d57d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d57d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d57d4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d57d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d57d4-106">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="d57d4-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="d57d4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d57d4-107">Methods</span></span>
|<span data-ttu-id="d57d4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d57d4-108">Method</span></span>|<span data-ttu-id="d57d4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d57d4-109">Return Type</span></span>|<span data-ttu-id="d57d4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d57d4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d57d4-111">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d57d4-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="d57d4-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d57d4-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="d57d4-113">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d57d4-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="d57d4-114">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d57d4-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="d57d4-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="d57d4-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="d57d4-116">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="d57d4-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="d57d4-117">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="d57d4-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="d57d4-118">Строка</span><span class="sxs-lookup"><span data-stu-id="d57d4-118">String</span></span>|<span data-ttu-id="d57d4-119">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="d57d4-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="d57d4-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="d57d4-120">Properties</span></span>
|<span data-ttu-id="d57d4-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="d57d4-121">Property</span></span>|<span data-ttu-id="d57d4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d57d4-122">Type</span></span>|<span data-ttu-id="d57d4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d57d4-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d57d4-124">id</span><span class="sxs-lookup"><span data-stu-id="d57d4-124">id</span></span>|<span data-ttu-id="d57d4-125">Строка</span><span class="sxs-lookup"><span data-stu-id="d57d4-125">String</span></span>|<span data-ttu-id="d57d4-126">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="d57d4-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="d57d4-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="d57d4-127">appleIdentifier</span></span>|<span data-ttu-id="d57d4-128">Строка</span><span class="sxs-lookup"><span data-stu-id="d57d4-128">String</span></span>|<span data-ttu-id="d57d4-129">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="d57d4-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="d57d4-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="d57d4-130">topicIdentifier</span></span>|<span data-ttu-id="d57d4-131">String</span><span class="sxs-lookup"><span data-stu-id="d57d4-131">String</span></span>|<span data-ttu-id="d57d4-132">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="d57d4-132">Topic Id.</span></span>|
|<span data-ttu-id="d57d4-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d57d4-133">lastModifiedDateTime</span></span>|<span data-ttu-id="d57d4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d57d4-134">DateTimeOffset</span></span>|<span data-ttu-id="d57d4-135">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="d57d4-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d57d4-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d57d4-136">expirationDateTime</span></span>|<span data-ttu-id="d57d4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d57d4-137">DateTimeOffset</span></span>|<span data-ttu-id="d57d4-138">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="d57d4-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="d57d4-139">certificate</span><span class="sxs-lookup"><span data-stu-id="d57d4-139">certificate</span></span>|<span data-ttu-id="d57d4-140">String</span><span class="sxs-lookup"><span data-stu-id="d57d4-140">String</span></span>|<span data-ttu-id="d57d4-141">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d57d4-141">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="d57d4-142">Связи</span><span class="sxs-lookup"><span data-stu-id="d57d4-142">Relationships</span></span>
<span data-ttu-id="d57d4-143">Нет</span><span class="sxs-lookup"><span data-stu-id="d57d4-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d57d4-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d57d4-144">JSON Representation</span></span>
<span data-ttu-id="d57d4-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d57d4-145">Here is a JSON representation of the resource.</span></span>
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




