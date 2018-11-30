---
title: Тип ресурса certificateConnectorSetting
description: Параметры соединителя сертификата.
ms.openlocfilehash: 65f87002016c4d5bd6b19106ba1aa988ad30d92e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074571"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="c6bfa-103">Тип ресурса certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="c6bfa-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="c6bfa-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6bfa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6bfa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6bfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6bfa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c6bfa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6bfa-107">Параметры соединителя сертификата.</span><span class="sxs-lookup"><span data-stu-id="c6bfa-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="c6bfa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6bfa-108">Properties</span></span>
|<span data-ttu-id="c6bfa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6bfa-109">Property</span></span>|<span data-ttu-id="c6bfa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c6bfa-110">Type</span></span>|<span data-ttu-id="c6bfa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c6bfa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6bfa-112">status</span><span class="sxs-lookup"><span data-stu-id="c6bfa-112">status</span></span>|<span data-ttu-id="c6bfa-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c6bfa-113">Int32</span></span>|<span data-ttu-id="c6bfa-114">Состояние соединителя сертификата</span><span class="sxs-lookup"><span data-stu-id="c6bfa-114">Certificate connector status</span></span>|
|<span data-ttu-id="c6bfa-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="c6bfa-115">certExpiryTime</span></span>|<span data-ttu-id="c6bfa-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6bfa-116">DateTimeOffset</span></span>|<span data-ttu-id="c6bfa-117">Срок действия сертификата времени</span><span class="sxs-lookup"><span data-stu-id="c6bfa-117">Certificate expire time</span></span>|
|<span data-ttu-id="c6bfa-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="c6bfa-118">enrollmentError</span></span>|<span data-ttu-id="c6bfa-119">String</span><span class="sxs-lookup"><span data-stu-id="c6bfa-119">String</span></span>|<span data-ttu-id="c6bfa-120">Ошибка регистрации сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="c6bfa-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="c6bfa-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="c6bfa-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="c6bfa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6bfa-122">DateTimeOffset</span></span>|<span data-ttu-id="c6bfa-123">Время последнего сертификата подключенных соединителя</span><span class="sxs-lookup"><span data-stu-id="c6bfa-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="c6bfa-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="c6bfa-124">connectorVersion</span></span>|<span data-ttu-id="c6bfa-125">String</span><span class="sxs-lookup"><span data-stu-id="c6bfa-125">String</span></span>|<span data-ttu-id="c6bfa-126">Версия сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="c6bfa-126">Version of certificate connector</span></span>|
|<span data-ttu-id="c6bfa-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="c6bfa-127">lastUploadVersion</span></span>|<span data-ttu-id="c6bfa-128">Int64</span><span class="sxs-lookup"><span data-stu-id="c6bfa-128">Int64</span></span>|<span data-ttu-id="c6bfa-129">Версия последнего загруженного сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="c6bfa-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6bfa-130">Связи</span><span class="sxs-lookup"><span data-stu-id="c6bfa-130">Relationships</span></span>
<span data-ttu-id="c6bfa-131">Нет</span><span class="sxs-lookup"><span data-stu-id="c6bfa-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6bfa-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6bfa-132">JSON Representation</span></span>
<span data-ttu-id="c6bfa-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6bfa-133">Here is a JSON representation of the resource.</span></span>
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





