---
title: Тип ресурса Цертификатеконнекторсеттинг
description: Параметры соединителя сертификатов.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60c7ac990a4eccd1f4faf0fd8f32c42a1e1addba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341986"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="49cd5-103">Тип ресурса Цертификатеконнекторсеттинг</span><span class="sxs-lookup"><span data-stu-id="49cd5-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="49cd5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49cd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49cd5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49cd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49cd5-106">Параметры соединителя сертификатов.</span><span class="sxs-lookup"><span data-stu-id="49cd5-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="49cd5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="49cd5-107">Properties</span></span>
|<span data-ttu-id="49cd5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="49cd5-108">Property</span></span>|<span data-ttu-id="49cd5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="49cd5-109">Type</span></span>|<span data-ttu-id="49cd5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="49cd5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49cd5-111">status</span><span class="sxs-lookup"><span data-stu-id="49cd5-111">status</span></span>|<span data-ttu-id="49cd5-112">Int32</span><span class="sxs-lookup"><span data-stu-id="49cd5-112">Int32</span></span>|<span data-ttu-id="49cd5-113">Состояние соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="49cd5-113">Certificate connector status</span></span>|
|<span data-ttu-id="49cd5-114">цертекспиритиме</span><span class="sxs-lookup"><span data-stu-id="49cd5-114">certExpiryTime</span></span>|<span data-ttu-id="49cd5-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cd5-115">DateTimeOffset</span></span>|<span data-ttu-id="49cd5-116">Время истечения срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="49cd5-116">Certificate expire time</span></span>|
|<span data-ttu-id="49cd5-117">енроллментеррор</span><span class="sxs-lookup"><span data-stu-id="49cd5-117">enrollmentError</span></span>|<span data-ttu-id="49cd5-118">String</span><span class="sxs-lookup"><span data-stu-id="49cd5-118">String</span></span>|<span data-ttu-id="49cd5-119">Ошибка регистрации соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="49cd5-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="49cd5-120">ластконнекторконнектионтиме</span><span class="sxs-lookup"><span data-stu-id="49cd5-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="49cd5-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cd5-121">DateTimeOffset</span></span>|<span data-ttu-id="49cd5-122">Время последнего подключения к соединителю сертификата</span><span class="sxs-lookup"><span data-stu-id="49cd5-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="49cd5-123">коннекторверсион</span><span class="sxs-lookup"><span data-stu-id="49cd5-123">connectorVersion</span></span>|<span data-ttu-id="49cd5-124">String</span><span class="sxs-lookup"><span data-stu-id="49cd5-124">String</span></span>|<span data-ttu-id="49cd5-125">Версия соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="49cd5-125">Version of certificate connector</span></span>|
|<span data-ttu-id="49cd5-126">ластуплоадверсион</span><span class="sxs-lookup"><span data-stu-id="49cd5-126">lastUploadVersion</span></span>|<span data-ttu-id="49cd5-127">Int64</span><span class="sxs-lookup"><span data-stu-id="49cd5-127">Int64</span></span>|<span data-ttu-id="49cd5-128">Версия последнего отправленного соединителя сертификатов</span><span class="sxs-lookup"><span data-stu-id="49cd5-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="49cd5-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="49cd5-129">Relationships</span></span>
<span data-ttu-id="49cd5-130">Нет</span><span class="sxs-lookup"><span data-stu-id="49cd5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49cd5-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49cd5-131">JSON Representation</span></span>
<span data-ttu-id="49cd5-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49cd5-132">Here is a JSON representation of the resource.</span></span>
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



