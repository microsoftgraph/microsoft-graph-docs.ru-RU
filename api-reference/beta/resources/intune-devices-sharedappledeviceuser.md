---
title: Тип ресурса Шаредаппледевицеусер
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f737432597d4528d1a682cd15552230af0ae83e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156506"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="139eb-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="139eb-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="139eb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="139eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="139eb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="139eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="139eb-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="139eb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="139eb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="139eb-107">Properties</span></span>
|<span data-ttu-id="139eb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="139eb-108">Property</span></span>|<span data-ttu-id="139eb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="139eb-109">Type</span></span>|<span data-ttu-id="139eb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="139eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="139eb-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="139eb-111">userPrincipalName</span></span>|<span data-ttu-id="139eb-112">String</span><span class="sxs-lookup"><span data-stu-id="139eb-112">String</span></span>|<span data-ttu-id="139eb-113">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="139eb-113">User name</span></span>|
|<span data-ttu-id="139eb-114">Дататосинк</span><span class="sxs-lookup"><span data-stu-id="139eb-114">dataToSync</span></span>|<span data-ttu-id="139eb-115">Логический</span><span class="sxs-lookup"><span data-stu-id="139eb-115">Boolean</span></span>|<span data-ttu-id="139eb-116">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="139eb-116">Data to sync</span></span>|
|<span data-ttu-id="139eb-117">Квота</span><span class="sxs-lookup"><span data-stu-id="139eb-117">dataQuota</span></span>|<span data-ttu-id="139eb-118">Int64</span><span class="sxs-lookup"><span data-stu-id="139eb-118">Int64</span></span>|<span data-ttu-id="139eb-119">Квота данных</span><span class="sxs-lookup"><span data-stu-id="139eb-119">Data quota</span></span>|
|<span data-ttu-id="139eb-120">Используется</span><span class="sxs-lookup"><span data-stu-id="139eb-120">dataUsed</span></span>|<span data-ttu-id="139eb-121">Int64</span><span class="sxs-lookup"><span data-stu-id="139eb-121">Int64</span></span>|<span data-ttu-id="139eb-122">Квота данных</span><span class="sxs-lookup"><span data-stu-id="139eb-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="139eb-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="139eb-123">Relationships</span></span>
<span data-ttu-id="139eb-124">Нет</span><span class="sxs-lookup"><span data-stu-id="139eb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="139eb-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="139eb-125">JSON Representation</span></span>
<span data-ttu-id="139eb-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="139eb-126">Here is a JSON representation of the resource.</span></span>
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




