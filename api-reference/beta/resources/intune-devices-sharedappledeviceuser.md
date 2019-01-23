---
title: Тип ресурса sharedAppleDeviceUser
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 46e0993c69a8ae34a54a654959d8d67a1b7f4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394434"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="fe449-103">Тип ресурса sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="fe449-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="fe449-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe449-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe449-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe449-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe449-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe449-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe449-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fe449-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fe449-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe449-108">Properties</span></span>
|<span data-ttu-id="fe449-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe449-109">Property</span></span>|<span data-ttu-id="fe449-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fe449-110">Type</span></span>|<span data-ttu-id="fe449-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe449-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe449-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe449-112">userPrincipalName</span></span>|<span data-ttu-id="fe449-113">String</span><span class="sxs-lookup"><span data-stu-id="fe449-113">String</span></span>|<span data-ttu-id="fe449-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="fe449-114">User name</span></span>|
|<span data-ttu-id="fe449-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="fe449-115">dataToSync</span></span>|<span data-ttu-id="fe449-116">Логический</span><span class="sxs-lookup"><span data-stu-id="fe449-116">Boolean</span></span>|<span data-ttu-id="fe449-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="fe449-117">Data to sync</span></span>|
|<span data-ttu-id="fe449-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="fe449-118">dataQuota</span></span>|<span data-ttu-id="fe449-119">Int64</span><span class="sxs-lookup"><span data-stu-id="fe449-119">Int64</span></span>|<span data-ttu-id="fe449-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="fe449-120">Data quota</span></span>|
|<span data-ttu-id="fe449-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="fe449-121">dataUsed</span></span>|<span data-ttu-id="fe449-122">Int64</span><span class="sxs-lookup"><span data-stu-id="fe449-122">Int64</span></span>|<span data-ttu-id="fe449-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="fe449-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe449-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="fe449-124">Relationships</span></span>
<span data-ttu-id="fe449-125">Нет</span><span class="sxs-lookup"><span data-stu-id="fe449-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe449-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe449-126">JSON Representation</span></span>
<span data-ttu-id="fe449-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe449-127">Here is a JSON representation of the resource.</span></span>
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




