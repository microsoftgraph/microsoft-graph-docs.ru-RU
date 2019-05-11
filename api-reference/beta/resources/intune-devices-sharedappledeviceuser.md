---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff51ad89600919fb1ed2c3bb506a53178ccdc445
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941753"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="b28fd-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="b28fd-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="b28fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b28fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b28fd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b28fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b28fd-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b28fd-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b28fd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b28fd-107">Properties</span></span>
|<span data-ttu-id="b28fd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b28fd-108">Property</span></span>|<span data-ttu-id="b28fd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b28fd-109">Type</span></span>|<span data-ttu-id="b28fd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b28fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b28fd-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b28fd-111">userPrincipalName</span></span>|<span data-ttu-id="b28fd-112">String</span><span class="sxs-lookup"><span data-stu-id="b28fd-112">String</span></span>|<span data-ttu-id="b28fd-113">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="b28fd-113">User name</span></span>|
|<span data-ttu-id="b28fd-114">Дататосинк</span><span class="sxs-lookup"><span data-stu-id="b28fd-114">dataToSync</span></span>|<span data-ttu-id="b28fd-115">Логический</span><span class="sxs-lookup"><span data-stu-id="b28fd-115">Boolean</span></span>|<span data-ttu-id="b28fd-116">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="b28fd-116">Data to sync</span></span>|
|<span data-ttu-id="b28fd-117">Квота</span><span class="sxs-lookup"><span data-stu-id="b28fd-117">dataQuota</span></span>|<span data-ttu-id="b28fd-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b28fd-118">Int64</span></span>|<span data-ttu-id="b28fd-119">Квота данных</span><span class="sxs-lookup"><span data-stu-id="b28fd-119">Data quota</span></span>|
|<span data-ttu-id="b28fd-120">Используется</span><span class="sxs-lookup"><span data-stu-id="b28fd-120">dataUsed</span></span>|<span data-ttu-id="b28fd-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b28fd-121">Int64</span></span>|<span data-ttu-id="b28fd-122">Квота данных</span><span class="sxs-lookup"><span data-stu-id="b28fd-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="b28fd-123">Связи</span><span class="sxs-lookup"><span data-stu-id="b28fd-123">Relationships</span></span>
<span data-ttu-id="b28fd-124">Нет</span><span class="sxs-lookup"><span data-stu-id="b28fd-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b28fd-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b28fd-125">JSON Representation</span></span>
<span data-ttu-id="b28fd-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b28fd-126">Here is a JSON representation of the resource.</span></span>
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




