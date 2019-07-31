---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c375b0c380cc719c8f49ba683a580133835e3a75
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968164"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="bebcb-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="bebcb-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="bebcb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bebcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bebcb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bebcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bebcb-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bebcb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bebcb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bebcb-107">Properties</span></span>
|<span data-ttu-id="bebcb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bebcb-108">Property</span></span>|<span data-ttu-id="bebcb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bebcb-109">Type</span></span>|<span data-ttu-id="bebcb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bebcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bebcb-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bebcb-111">userPrincipalName</span></span>|<span data-ttu-id="bebcb-112">String</span><span class="sxs-lookup"><span data-stu-id="bebcb-112">String</span></span>|<span data-ttu-id="bebcb-113">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="bebcb-113">User name</span></span>|
|<span data-ttu-id="bebcb-114">Дататосинк</span><span class="sxs-lookup"><span data-stu-id="bebcb-114">dataToSync</span></span>|<span data-ttu-id="bebcb-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bebcb-115">Boolean</span></span>|<span data-ttu-id="bebcb-116">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="bebcb-116">Data to sync</span></span>|
|<span data-ttu-id="bebcb-117">Квота</span><span class="sxs-lookup"><span data-stu-id="bebcb-117">dataQuota</span></span>|<span data-ttu-id="bebcb-118">Int64</span><span class="sxs-lookup"><span data-stu-id="bebcb-118">Int64</span></span>|<span data-ttu-id="bebcb-119">Квота данных</span><span class="sxs-lookup"><span data-stu-id="bebcb-119">Data quota</span></span>|
|<span data-ttu-id="bebcb-120">Используется</span><span class="sxs-lookup"><span data-stu-id="bebcb-120">dataUsed</span></span>|<span data-ttu-id="bebcb-121">Int64</span><span class="sxs-lookup"><span data-stu-id="bebcb-121">Int64</span></span>|<span data-ttu-id="bebcb-122">Квота данных</span><span class="sxs-lookup"><span data-stu-id="bebcb-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="bebcb-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="bebcb-123">Relationships</span></span>
<span data-ttu-id="bebcb-124">Нет</span><span class="sxs-lookup"><span data-stu-id="bebcb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bebcb-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bebcb-125">JSON Representation</span></span>
<span data-ttu-id="bebcb-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bebcb-126">Here is a JSON representation of the resource.</span></span>
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





