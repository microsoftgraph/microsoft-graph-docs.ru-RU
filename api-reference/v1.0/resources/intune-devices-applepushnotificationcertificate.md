---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c56f78a596d08037ca68a96bf9cc5aca5fbf148
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027505"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="00d1c-103">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="00d1c-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="00d1c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00d1c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00d1c-105">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="00d1c-105">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="00d1c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="00d1c-106">Methods</span></span>
|<span data-ttu-id="00d1c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="00d1c-107">Method</span></span>|<span data-ttu-id="00d1c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="00d1c-108">Return Type</span></span>|<span data-ttu-id="00d1c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="00d1c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00d1c-110">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="00d1c-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="00d1c-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="00d1c-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="00d1c-112">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="00d1c-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="00d1c-113">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="00d1c-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="00d1c-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="00d1c-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="00d1c-115">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="00d1c-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="00d1c-116">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="00d1c-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="00d1c-117">String</span><span class="sxs-lookup"><span data-stu-id="00d1c-117">String</span></span>|<span data-ttu-id="00d1c-118">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="00d1c-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="00d1c-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="00d1c-119">Properties</span></span>
|<span data-ttu-id="00d1c-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="00d1c-120">Property</span></span>|<span data-ttu-id="00d1c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="00d1c-121">Type</span></span>|<span data-ttu-id="00d1c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="00d1c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00d1c-123">id</span><span class="sxs-lookup"><span data-stu-id="00d1c-123">id</span></span>|<span data-ttu-id="00d1c-124">String</span><span class="sxs-lookup"><span data-stu-id="00d1c-124">String</span></span>|<span data-ttu-id="00d1c-125">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="00d1c-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="00d1c-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="00d1c-126">appleIdentifier</span></span>|<span data-ttu-id="00d1c-127">String</span><span class="sxs-lookup"><span data-stu-id="00d1c-127">String</span></span>|<span data-ttu-id="00d1c-128">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="00d1c-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="00d1c-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="00d1c-129">topicIdentifier</span></span>|<span data-ttu-id="00d1c-130">String</span><span class="sxs-lookup"><span data-stu-id="00d1c-130">String</span></span>|<span data-ttu-id="00d1c-131">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="00d1c-131">Topic Id.</span></span>|
|<span data-ttu-id="00d1c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00d1c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="00d1c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d1c-133">DateTimeOffset</span></span>|<span data-ttu-id="00d1c-134">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="00d1c-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="00d1c-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="00d1c-135">expirationDateTime</span></span>|<span data-ttu-id="00d1c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00d1c-136">DateTimeOffset</span></span>|<span data-ttu-id="00d1c-137">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="00d1c-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="00d1c-138">certificate</span><span class="sxs-lookup"><span data-stu-id="00d1c-138">certificate</span></span>|<span data-ttu-id="00d1c-139">String</span><span class="sxs-lookup"><span data-stu-id="00d1c-139">String</span></span>|<span data-ttu-id="00d1c-140">Н/Д</span><span class="sxs-lookup"><span data-stu-id="00d1c-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="00d1c-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="00d1c-141">Relationships</span></span>
<span data-ttu-id="00d1c-142">Нет</span><span class="sxs-lookup"><span data-stu-id="00d1c-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00d1c-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00d1c-143">JSON Representation</span></span>
<span data-ttu-id="00d1c-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00d1c-144">Here is a JSON representation of the resource.</span></span>
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



