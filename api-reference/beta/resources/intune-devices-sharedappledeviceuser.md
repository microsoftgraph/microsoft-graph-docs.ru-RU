---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 550d8af3cab51f611feed7f87f1d2f56a850de4e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783860"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="ffa3e-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="ffa3e-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="ffa3e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffa3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffa3e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffa3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffa3e-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ffa3e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ffa3e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffa3e-107">Properties</span></span>
|<span data-ttu-id="ffa3e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffa3e-108">Property</span></span>|<span data-ttu-id="ffa3e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ffa3e-109">Type</span></span>|<span data-ttu-id="ffa3e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ffa3e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffa3e-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ffa3e-111">userPrincipalName</span></span>|<span data-ttu-id="ffa3e-112">String</span><span class="sxs-lookup"><span data-stu-id="ffa3e-112">String</span></span>|<span data-ttu-id="ffa3e-113">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="ffa3e-113">User name</span></span>|
|<span data-ttu-id="ffa3e-114">дататосинк</span><span class="sxs-lookup"><span data-stu-id="ffa3e-114">dataToSync</span></span>|<span data-ttu-id="ffa3e-115">Логический</span><span class="sxs-lookup"><span data-stu-id="ffa3e-115">Boolean</span></span>|<span data-ttu-id="ffa3e-116">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="ffa3e-116">Data to sync</span></span>|
|<span data-ttu-id="ffa3e-117">Квота</span><span class="sxs-lookup"><span data-stu-id="ffa3e-117">dataQuota</span></span>|<span data-ttu-id="ffa3e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ffa3e-118">Int64</span></span>|<span data-ttu-id="ffa3e-119">Квота данных</span><span class="sxs-lookup"><span data-stu-id="ffa3e-119">Data quota</span></span>|
|<span data-ttu-id="ffa3e-120">Используется</span><span class="sxs-lookup"><span data-stu-id="ffa3e-120">dataUsed</span></span>|<span data-ttu-id="ffa3e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ffa3e-121">Int64</span></span>|<span data-ttu-id="ffa3e-122">Квота данных</span><span class="sxs-lookup"><span data-stu-id="ffa3e-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffa3e-123">Связи</span><span class="sxs-lookup"><span data-stu-id="ffa3e-123">Relationships</span></span>
<span data-ttu-id="ffa3e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="ffa3e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffa3e-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffa3e-125">JSON Representation</span></span>
<span data-ttu-id="ffa3e-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffa3e-126">Here is a JSON representation of the resource.</span></span>
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



