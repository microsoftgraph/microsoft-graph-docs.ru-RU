---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4cd33eccfbc1c3e396d65f63a6f435690186b53f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208795"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="3d9a5-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="3d9a5-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="3d9a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d9a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d9a5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d9a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d9a5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d9a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d9a5-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3d9a5-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3d9a5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d9a5-108">Properties</span></span>
|<span data-ttu-id="3d9a5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d9a5-109">Property</span></span>|<span data-ttu-id="3d9a5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3d9a5-110">Type</span></span>|<span data-ttu-id="3d9a5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3d9a5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d9a5-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3d9a5-112">userPrincipalName</span></span>|<span data-ttu-id="3d9a5-113">String</span><span class="sxs-lookup"><span data-stu-id="3d9a5-113">String</span></span>|<span data-ttu-id="3d9a5-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="3d9a5-114">User name</span></span>|
|<span data-ttu-id="3d9a5-115">дататосинк</span><span class="sxs-lookup"><span data-stu-id="3d9a5-115">dataToSync</span></span>|<span data-ttu-id="3d9a5-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d9a5-116">Boolean</span></span>|<span data-ttu-id="3d9a5-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="3d9a5-117">Data to sync</span></span>|
|<span data-ttu-id="3d9a5-118">Квота</span><span class="sxs-lookup"><span data-stu-id="3d9a5-118">dataQuota</span></span>|<span data-ttu-id="3d9a5-119">Int64</span><span class="sxs-lookup"><span data-stu-id="3d9a5-119">Int64</span></span>|<span data-ttu-id="3d9a5-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="3d9a5-120">Data quota</span></span>|
|<span data-ttu-id="3d9a5-121">Используется</span><span class="sxs-lookup"><span data-stu-id="3d9a5-121">dataUsed</span></span>|<span data-ttu-id="3d9a5-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3d9a5-122">Int64</span></span>|<span data-ttu-id="3d9a5-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="3d9a5-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d9a5-124">Связи</span><span class="sxs-lookup"><span data-stu-id="3d9a5-124">Relationships</span></span>
<span data-ttu-id="3d9a5-125">Нет</span><span class="sxs-lookup"><span data-stu-id="3d9a5-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d9a5-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d9a5-126">JSON Representation</span></span>
<span data-ttu-id="3d9a5-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d9a5-127">Here is a JSON representation of the resource.</span></span>
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




