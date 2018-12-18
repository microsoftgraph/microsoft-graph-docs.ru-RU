---
title: Тип ресурса certificateConnectorSetting
description: Параметры соединителя сертификата.
author: tfitzmac
ms.openlocfilehash: 8c993634eb4f41e16643ae3f40be74ecc3eb392f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326308"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="f1978-103">Тип ресурса certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f1978-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="f1978-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1978-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1978-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1978-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1978-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1978-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1978-107">Параметры соединителя сертификата.</span><span class="sxs-lookup"><span data-stu-id="f1978-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="f1978-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1978-108">Properties</span></span>
|<span data-ttu-id="f1978-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1978-109">Property</span></span>|<span data-ttu-id="f1978-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f1978-110">Type</span></span>|<span data-ttu-id="f1978-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f1978-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1978-112">status</span><span class="sxs-lookup"><span data-stu-id="f1978-112">status</span></span>|<span data-ttu-id="f1978-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f1978-113">Int32</span></span>|<span data-ttu-id="f1978-114">Состояние соединителя сертификата</span><span class="sxs-lookup"><span data-stu-id="f1978-114">Certificate connector status</span></span>|
|<span data-ttu-id="f1978-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="f1978-115">certExpiryTime</span></span>|<span data-ttu-id="f1978-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1978-116">DateTimeOffset</span></span>|<span data-ttu-id="f1978-117">Срок действия сертификата времени</span><span class="sxs-lookup"><span data-stu-id="f1978-117">Certificate expire time</span></span>|
|<span data-ttu-id="f1978-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="f1978-118">enrollmentError</span></span>|<span data-ttu-id="f1978-119">String.</span><span class="sxs-lookup"><span data-stu-id="f1978-119">String</span></span>|<span data-ttu-id="f1978-120">Ошибка регистрации сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="f1978-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="f1978-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="f1978-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="f1978-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1978-122">DateTimeOffset</span></span>|<span data-ttu-id="f1978-123">Время последнего сертификата подключенных соединителя</span><span class="sxs-lookup"><span data-stu-id="f1978-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="f1978-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="f1978-124">connectorVersion</span></span>|<span data-ttu-id="f1978-125">String.</span><span class="sxs-lookup"><span data-stu-id="f1978-125">String</span></span>|<span data-ttu-id="f1978-126">Версия сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="f1978-126">Version of certificate connector</span></span>|
|<span data-ttu-id="f1978-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="f1978-127">lastUploadVersion</span></span>|<span data-ttu-id="f1978-128">Int64</span><span class="sxs-lookup"><span data-stu-id="f1978-128">Int64</span></span>|<span data-ttu-id="f1978-129">Версия последнего загруженного сертификата соединителя</span><span class="sxs-lookup"><span data-stu-id="f1978-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1978-130">Связи</span><span class="sxs-lookup"><span data-stu-id="f1978-130">Relationships</span></span>
<span data-ttu-id="f1978-131">Нет</span><span class="sxs-lookup"><span data-stu-id="f1978-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1978-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1978-132">JSON Representation</span></span>
<span data-ttu-id="f1978-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1978-133">Here is a JSON representation of the resource.</span></span>
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





