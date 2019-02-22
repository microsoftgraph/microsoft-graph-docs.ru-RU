---
title: Тип ресурса Цертификатеконнекторсеттинг
description: Параметры соединителя сертификатов.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09f4baf9ddd8be630c432fcec5d7df71c442bbe2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168308"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="5d800-103">Тип ресурса Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="5d800-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="5d800-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d800-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d800-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d800-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d800-106">Параметры соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="5d800-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="5d800-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d800-107">Properties</span></span>
|<span data-ttu-id="5d800-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d800-108">Property</span></span>|<span data-ttu-id="5d800-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5d800-109">Type</span></span>|<span data-ttu-id="5d800-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d800-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d800-111">status</span><span class="sxs-lookup"><span data-stu-id="5d800-111">status</span></span>|<span data-ttu-id="5d800-112">Int32</span><span class="sxs-lookup"><span data-stu-id="5d800-112">Int32</span></span>|<span data-ttu-id="5d800-113">Состояние соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="5d800-113">Certificate connector status</span></span>|
|<span data-ttu-id="5d800-114">Цертекспиритиме</span><span class="sxs-lookup"><span data-stu-id="5d800-114">certExpiryTime</span></span>|<span data-ttu-id="5d800-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d800-115">DateTimeOffset</span></span>|<span data-ttu-id="5d800-116">Время истечения срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="5d800-116">Certificate expire time</span></span>|
|<span data-ttu-id="5d800-117">Енроллментеррор</span><span class="sxs-lookup"><span data-stu-id="5d800-117">enrollmentError</span></span>|<span data-ttu-id="5d800-118">String</span><span class="sxs-lookup"><span data-stu-id="5d800-118">String</span></span>|<span data-ttu-id="5d800-119">Ошибка регистрации соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="5d800-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="5d800-120">Ластконнекторконнектионтиме</span><span class="sxs-lookup"><span data-stu-id="5d800-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="5d800-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d800-121">DateTimeOffset</span></span>|<span data-ttu-id="5d800-122">Время последнего подключения к соединителю сертификата</span><span class="sxs-lookup"><span data-stu-id="5d800-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="5d800-123">Коннекторверсион</span><span class="sxs-lookup"><span data-stu-id="5d800-123">connectorVersion</span></span>|<span data-ttu-id="5d800-124">String</span><span class="sxs-lookup"><span data-stu-id="5d800-124">String</span></span>|<span data-ttu-id="5d800-125">Версия соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="5d800-125">Version of certificate connector</span></span>|
|<span data-ttu-id="5d800-126">Ластуплоадверсион</span><span class="sxs-lookup"><span data-stu-id="5d800-126">lastUploadVersion</span></span>|<span data-ttu-id="5d800-127">Int64</span><span class="sxs-lookup"><span data-stu-id="5d800-127">Int64</span></span>|<span data-ttu-id="5d800-128">Версия последнего отправленного соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="5d800-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d800-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="5d800-129">Relationships</span></span>
<span data-ttu-id="5d800-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5d800-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d800-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d800-131">JSON Representation</span></span>
<span data-ttu-id="5d800-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d800-132">Here is a JSON representation of the resource.</span></span>
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




