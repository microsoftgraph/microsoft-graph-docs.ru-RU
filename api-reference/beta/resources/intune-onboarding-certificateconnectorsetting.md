---
title: Тип ресурса certificateConnectorSetting
description: Параметры соединителя сертификата.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5886418aaddede43f2397ad626028598a63a0066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398655"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="f21ba-103">Тип ресурса certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f21ba-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="f21ba-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f21ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f21ba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f21ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f21ba-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f21ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f21ba-107">Параметры соединителя сертификата.</span><span class="sxs-lookup"><span data-stu-id="f21ba-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="f21ba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f21ba-108">Properties</span></span>
|<span data-ttu-id="f21ba-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f21ba-109">Property</span></span>|<span data-ttu-id="f21ba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f21ba-110">Type</span></span>|<span data-ttu-id="f21ba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f21ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f21ba-112">status</span><span class="sxs-lookup"><span data-stu-id="f21ba-112">status</span></span>|<span data-ttu-id="f21ba-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f21ba-113">Int32</span></span>|<span data-ttu-id="f21ba-114">Состояние соединителя сертификата</span><span class="sxs-lookup"><span data-stu-id="f21ba-114">Certificate connector status</span></span>|
|<span data-ttu-id="f21ba-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="f21ba-115">certExpiryTime</span></span>|<span data-ttu-id="f21ba-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f21ba-116">DateTimeOffset</span></span>|<span data-ttu-id="f21ba-117">Срок действия сертификата времени</span><span class="sxs-lookup"><span data-stu-id="f21ba-117">Certificate expire time</span></span>|
|<span data-ttu-id="f21ba-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="f21ba-118">enrollmentError</span></span>|<span data-ttu-id="f21ba-119">String</span><span class="sxs-lookup"><span data-stu-id="f21ba-119">String</span></span>|<span data-ttu-id="f21ba-120">Ошибка регистрации сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="f21ba-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="f21ba-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="f21ba-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="f21ba-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f21ba-122">DateTimeOffset</span></span>|<span data-ttu-id="f21ba-123">Время последнего сертификата подключенных соединителя</span><span class="sxs-lookup"><span data-stu-id="f21ba-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="f21ba-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="f21ba-124">connectorVersion</span></span>|<span data-ttu-id="f21ba-125">String</span><span class="sxs-lookup"><span data-stu-id="f21ba-125">String</span></span>|<span data-ttu-id="f21ba-126">Версия сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="f21ba-126">Version of certificate connector</span></span>|
|<span data-ttu-id="f21ba-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="f21ba-127">lastUploadVersion</span></span>|<span data-ttu-id="f21ba-128">Int64</span><span class="sxs-lookup"><span data-stu-id="f21ba-128">Int64</span></span>|<span data-ttu-id="f21ba-129">Версия последнего загруженного сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="f21ba-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="f21ba-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="f21ba-130">Relationships</span></span>
<span data-ttu-id="f21ba-131">Нет</span><span class="sxs-lookup"><span data-stu-id="f21ba-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f21ba-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f21ba-132">JSON Representation</span></span>
<span data-ttu-id="f21ba-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f21ba-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```




