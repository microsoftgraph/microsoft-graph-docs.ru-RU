---
title: Тип ресурса certificateConnectorSetting
description: Параметры соединителя сертификата.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56f12600b6aa78982dc51732d685dcd7c962d0b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888601"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="39d87-103">Тип ресурса certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="39d87-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="39d87-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39d87-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39d87-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39d87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39d87-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="39d87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39d87-107">Параметры соединителя сертификата.</span><span class="sxs-lookup"><span data-stu-id="39d87-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="39d87-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="39d87-108">Properties</span></span>
|<span data-ttu-id="39d87-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="39d87-109">Property</span></span>|<span data-ttu-id="39d87-110">Тип</span><span class="sxs-lookup"><span data-stu-id="39d87-110">Type</span></span>|<span data-ttu-id="39d87-111">Описание</span><span class="sxs-lookup"><span data-stu-id="39d87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39d87-112">status</span><span class="sxs-lookup"><span data-stu-id="39d87-112">status</span></span>|<span data-ttu-id="39d87-113">Int32</span><span class="sxs-lookup"><span data-stu-id="39d87-113">Int32</span></span>|<span data-ttu-id="39d87-114">Состояние соединителя сертификата</span><span class="sxs-lookup"><span data-stu-id="39d87-114">Certificate connector status</span></span>|
|<span data-ttu-id="39d87-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="39d87-115">certExpiryTime</span></span>|<span data-ttu-id="39d87-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39d87-116">DateTimeOffset</span></span>|<span data-ttu-id="39d87-117">Срок действия сертификата времени</span><span class="sxs-lookup"><span data-stu-id="39d87-117">Certificate expire time</span></span>|
|<span data-ttu-id="39d87-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="39d87-118">enrollmentError</span></span>|<span data-ttu-id="39d87-119">Строка</span><span class="sxs-lookup"><span data-stu-id="39d87-119">String</span></span>|<span data-ttu-id="39d87-120">Ошибка регистрации сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="39d87-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="39d87-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="39d87-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="39d87-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39d87-122">DateTimeOffset</span></span>|<span data-ttu-id="39d87-123">Время последнего сертификата подключенных соединителя</span><span class="sxs-lookup"><span data-stu-id="39d87-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="39d87-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="39d87-124">connectorVersion</span></span>|<span data-ttu-id="39d87-125">Строка</span><span class="sxs-lookup"><span data-stu-id="39d87-125">String</span></span>|<span data-ttu-id="39d87-126">Версия сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="39d87-126">Version of certificate connector</span></span>|
|<span data-ttu-id="39d87-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="39d87-127">lastUploadVersion</span></span>|<span data-ttu-id="39d87-128">Int64</span><span class="sxs-lookup"><span data-stu-id="39d87-128">Int64</span></span>|<span data-ttu-id="39d87-129">Версия последнего загруженного сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="39d87-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="39d87-130">Связи</span><span class="sxs-lookup"><span data-stu-id="39d87-130">Relationships</span></span>
<span data-ttu-id="39d87-131">Нет</span><span class="sxs-lookup"><span data-stu-id="39d87-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39d87-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39d87-132">JSON Representation</span></span>
<span data-ttu-id="39d87-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39d87-133">Here is a JSON representation of the resource.</span></span>
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





