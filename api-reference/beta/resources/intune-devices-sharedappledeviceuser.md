---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df9f47aa4655c0e360d5c89f38443f5f8dc499ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081008"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="dba4e-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="dba4e-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="dba4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dba4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dba4e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dba4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dba4e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dba4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dba4e-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dba4e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="dba4e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dba4e-108">Properties</span></span>
|<span data-ttu-id="dba4e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dba4e-109">Property</span></span>|<span data-ttu-id="dba4e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dba4e-110">Type</span></span>|<span data-ttu-id="dba4e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dba4e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dba4e-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dba4e-112">userPrincipalName</span></span>|<span data-ttu-id="dba4e-113">String</span><span class="sxs-lookup"><span data-stu-id="dba4e-113">String</span></span>|<span data-ttu-id="dba4e-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="dba4e-114">User name</span></span>|
|<span data-ttu-id="dba4e-115">дататосинк</span><span class="sxs-lookup"><span data-stu-id="dba4e-115">dataToSync</span></span>|<span data-ttu-id="dba4e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba4e-116">Boolean</span></span>|<span data-ttu-id="dba4e-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="dba4e-117">Data to sync</span></span>|
|<span data-ttu-id="dba4e-118">Квота</span><span class="sxs-lookup"><span data-stu-id="dba4e-118">dataQuota</span></span>|<span data-ttu-id="dba4e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="dba4e-119">Int64</span></span>|<span data-ttu-id="dba4e-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="dba4e-120">Data quota</span></span>|
|<span data-ttu-id="dba4e-121">Используется</span><span class="sxs-lookup"><span data-stu-id="dba4e-121">dataUsed</span></span>|<span data-ttu-id="dba4e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="dba4e-122">Int64</span></span>|<span data-ttu-id="dba4e-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="dba4e-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="dba4e-124">Связи</span><span class="sxs-lookup"><span data-stu-id="dba4e-124">Relationships</span></span>
<span data-ttu-id="dba4e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="dba4e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dba4e-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dba4e-126">JSON Representation</span></span>
<span data-ttu-id="dba4e-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dba4e-127">Here is a JSON representation of the resource.</span></span>
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






