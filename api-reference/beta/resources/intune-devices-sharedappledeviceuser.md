---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3946247ba9424fb1c961a11753376b7bcfb78c4a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724454"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="6e9ba-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="6e9ba-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="6e9ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e9ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e9ba-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e9ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e9ba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e9ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e9ba-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6e9ba-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6e9ba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e9ba-108">Properties</span></span>
|<span data-ttu-id="6e9ba-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e9ba-109">Property</span></span>|<span data-ttu-id="6e9ba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6e9ba-110">Type</span></span>|<span data-ttu-id="6e9ba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6e9ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e9ba-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6e9ba-112">userPrincipalName</span></span>|<span data-ttu-id="6e9ba-113">String</span><span class="sxs-lookup"><span data-stu-id="6e9ba-113">String</span></span>|<span data-ttu-id="6e9ba-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="6e9ba-114">User name</span></span>|
|<span data-ttu-id="6e9ba-115">дататосинк</span><span class="sxs-lookup"><span data-stu-id="6e9ba-115">dataToSync</span></span>|<span data-ttu-id="6e9ba-116">Логический</span><span class="sxs-lookup"><span data-stu-id="6e9ba-116">Boolean</span></span>|<span data-ttu-id="6e9ba-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="6e9ba-117">Data to sync</span></span>|
|<span data-ttu-id="6e9ba-118">Квота</span><span class="sxs-lookup"><span data-stu-id="6e9ba-118">dataQuota</span></span>|<span data-ttu-id="6e9ba-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6e9ba-119">Int64</span></span>|<span data-ttu-id="6e9ba-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="6e9ba-120">Data quota</span></span>|
|<span data-ttu-id="6e9ba-121">Используется</span><span class="sxs-lookup"><span data-stu-id="6e9ba-121">dataUsed</span></span>|<span data-ttu-id="6e9ba-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6e9ba-122">Int64</span></span>|<span data-ttu-id="6e9ba-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="6e9ba-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e9ba-124">Связи</span><span class="sxs-lookup"><span data-stu-id="6e9ba-124">Relationships</span></span>
<span data-ttu-id="6e9ba-125">Нет</span><span class="sxs-lookup"><span data-stu-id="6e9ba-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e9ba-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e9ba-126">JSON Representation</span></span>
<span data-ttu-id="6e9ba-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e9ba-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```





