---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3d6142b47205640e64b8e422b1727fdf60ac8a2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524916"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="42375-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="42375-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="42375-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="42375-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42375-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42375-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42375-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42375-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42375-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="42375-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="42375-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="42375-108">Properties</span></span>
|<span data-ttu-id="42375-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="42375-109">Property</span></span>|<span data-ttu-id="42375-110">Тип</span><span class="sxs-lookup"><span data-stu-id="42375-110">Type</span></span>|<span data-ttu-id="42375-111">Описание</span><span class="sxs-lookup"><span data-stu-id="42375-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42375-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42375-112">userPrincipalName</span></span>|<span data-ttu-id="42375-113">String</span><span class="sxs-lookup"><span data-stu-id="42375-113">String</span></span>|<span data-ttu-id="42375-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="42375-114">User name</span></span>|
|<span data-ttu-id="42375-115">дататосинк</span><span class="sxs-lookup"><span data-stu-id="42375-115">dataToSync</span></span>|<span data-ttu-id="42375-116">Логический</span><span class="sxs-lookup"><span data-stu-id="42375-116">Boolean</span></span>|<span data-ttu-id="42375-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="42375-117">Data to sync</span></span>|
|<span data-ttu-id="42375-118">Квота</span><span class="sxs-lookup"><span data-stu-id="42375-118">dataQuota</span></span>|<span data-ttu-id="42375-119">Int64</span><span class="sxs-lookup"><span data-stu-id="42375-119">Int64</span></span>|<span data-ttu-id="42375-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="42375-120">Data quota</span></span>|
|<span data-ttu-id="42375-121">Используется</span><span class="sxs-lookup"><span data-stu-id="42375-121">dataUsed</span></span>|<span data-ttu-id="42375-122">Int64</span><span class="sxs-lookup"><span data-stu-id="42375-122">Int64</span></span>|<span data-ttu-id="42375-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="42375-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="42375-124">Связи</span><span class="sxs-lookup"><span data-stu-id="42375-124">Relationships</span></span>
<span data-ttu-id="42375-125">Нет</span><span class="sxs-lookup"><span data-stu-id="42375-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42375-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42375-126">JSON Representation</span></span>
<span data-ttu-id="42375-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42375-127">Here is a JSON representation of the resource.</span></span>
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



