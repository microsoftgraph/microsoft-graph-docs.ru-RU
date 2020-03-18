---
title: Тип ресурса Цертификатеконнекторсеттинг
description: Параметры соединителя сертификатов.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3230a5b512ab09b8b3c033f95c3fc7682197ff4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779879"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="1d921-103">Тип ресурса Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="1d921-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="1d921-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d921-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d921-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d921-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d921-106">Параметры соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="1d921-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="1d921-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d921-107">Properties</span></span>
|<span data-ttu-id="1d921-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d921-108">Property</span></span>|<span data-ttu-id="1d921-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1d921-109">Type</span></span>|<span data-ttu-id="1d921-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1d921-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d921-111">status</span><span class="sxs-lookup"><span data-stu-id="1d921-111">status</span></span>|<span data-ttu-id="1d921-112">Int32</span><span class="sxs-lookup"><span data-stu-id="1d921-112">Int32</span></span>|<span data-ttu-id="1d921-113">Состояние соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="1d921-113">Certificate connector status</span></span>|
|<span data-ttu-id="1d921-114">цертекспиритиме</span><span class="sxs-lookup"><span data-stu-id="1d921-114">certExpiryTime</span></span>|<span data-ttu-id="1d921-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d921-115">DateTimeOffset</span></span>|<span data-ttu-id="1d921-116">Время истечения срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="1d921-116">Certificate expire time</span></span>|
|<span data-ttu-id="1d921-117">енроллментеррор</span><span class="sxs-lookup"><span data-stu-id="1d921-117">enrollmentError</span></span>|<span data-ttu-id="1d921-118">String</span><span class="sxs-lookup"><span data-stu-id="1d921-118">String</span></span>|<span data-ttu-id="1d921-119">Ошибка регистрации соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="1d921-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="1d921-120">ластконнекторконнектионтиме</span><span class="sxs-lookup"><span data-stu-id="1d921-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="1d921-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d921-121">DateTimeOffset</span></span>|<span data-ttu-id="1d921-122">Время последнего подключения к соединителю сертификата</span><span class="sxs-lookup"><span data-stu-id="1d921-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="1d921-123">коннекторверсион</span><span class="sxs-lookup"><span data-stu-id="1d921-123">connectorVersion</span></span>|<span data-ttu-id="1d921-124">String</span><span class="sxs-lookup"><span data-stu-id="1d921-124">String</span></span>|<span data-ttu-id="1d921-125">Версия соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="1d921-125">Version of certificate connector</span></span>|
|<span data-ttu-id="1d921-126">ластуплоадверсион</span><span class="sxs-lookup"><span data-stu-id="1d921-126">lastUploadVersion</span></span>|<span data-ttu-id="1d921-127">Int64</span><span class="sxs-lookup"><span data-stu-id="1d921-127">Int64</span></span>|<span data-ttu-id="1d921-128">Версия последнего отправленного соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="1d921-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d921-129">Связи</span><span class="sxs-lookup"><span data-stu-id="1d921-129">Relationships</span></span>
<span data-ttu-id="1d921-130">Нет</span><span class="sxs-lookup"><span data-stu-id="1d921-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d921-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d921-131">JSON Representation</span></span>
<span data-ttu-id="1d921-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d921-132">Here is a JSON representation of the resource.</span></span>
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



