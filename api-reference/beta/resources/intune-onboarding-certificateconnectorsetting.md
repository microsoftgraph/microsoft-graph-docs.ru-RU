---
title: Тип ресурса Цертификатеконнекторсеттинг
description: Параметры соединителя сертификатов.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 969edd445e293d7417f2bf08c7641844b1ddffff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419047"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="bc252-103">Тип ресурса Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="bc252-103">certificateConnectorSetting resource type</span></span>

<span data-ttu-id="bc252-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc252-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc252-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc252-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc252-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc252-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc252-107">Параметры соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bc252-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="bc252-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc252-108">Properties</span></span>
|<span data-ttu-id="bc252-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc252-109">Property</span></span>|<span data-ttu-id="bc252-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bc252-110">Type</span></span>|<span data-ttu-id="bc252-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bc252-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc252-112">status</span><span class="sxs-lookup"><span data-stu-id="bc252-112">status</span></span>|<span data-ttu-id="bc252-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bc252-113">Int32</span></span>|<span data-ttu-id="bc252-114">Состояние соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="bc252-114">Certificate connector status</span></span>|
|<span data-ttu-id="bc252-115">цертекспиритиме</span><span class="sxs-lookup"><span data-stu-id="bc252-115">certExpiryTime</span></span>|<span data-ttu-id="bc252-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc252-116">DateTimeOffset</span></span>|<span data-ttu-id="bc252-117">Время истечения срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="bc252-117">Certificate expire time</span></span>|
|<span data-ttu-id="bc252-118">енроллментеррор</span><span class="sxs-lookup"><span data-stu-id="bc252-118">enrollmentError</span></span>|<span data-ttu-id="bc252-119">String</span><span class="sxs-lookup"><span data-stu-id="bc252-119">String</span></span>|<span data-ttu-id="bc252-120">Ошибка регистрации соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="bc252-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="bc252-121">ластконнекторконнектионтиме</span><span class="sxs-lookup"><span data-stu-id="bc252-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="bc252-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc252-122">DateTimeOffset</span></span>|<span data-ttu-id="bc252-123">Время последнего подключения к соединителю сертификата</span><span class="sxs-lookup"><span data-stu-id="bc252-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="bc252-124">коннекторверсион</span><span class="sxs-lookup"><span data-stu-id="bc252-124">connectorVersion</span></span>|<span data-ttu-id="bc252-125">String</span><span class="sxs-lookup"><span data-stu-id="bc252-125">String</span></span>|<span data-ttu-id="bc252-126">Версия соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="bc252-126">Version of certificate connector</span></span>|
|<span data-ttu-id="bc252-127">ластуплоадверсион</span><span class="sxs-lookup"><span data-stu-id="bc252-127">lastUploadVersion</span></span>|<span data-ttu-id="bc252-128">Int64</span><span class="sxs-lookup"><span data-stu-id="bc252-128">Int64</span></span>|<span data-ttu-id="bc252-129">Версия последнего отправленного соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="bc252-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc252-130">Связи</span><span class="sxs-lookup"><span data-stu-id="bc252-130">Relationships</span></span>
<span data-ttu-id="bc252-131">Нет</span><span class="sxs-lookup"><span data-stu-id="bc252-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc252-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc252-132">JSON Representation</span></span>
<span data-ttu-id="bc252-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc252-133">Here is a JSON representation of the resource.</span></span>
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



