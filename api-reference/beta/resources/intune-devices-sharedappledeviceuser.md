---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4dc78ad66302d4ffd330936cc95bd9b3cd7ae900
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383052"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="d747a-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="d747a-103">sharedAppleDeviceUser resource type</span></span>

<span data-ttu-id="d747a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d747a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d747a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d747a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d747a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d747a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d747a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d747a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d747a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d747a-108">Properties</span></span>
|<span data-ttu-id="d747a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d747a-109">Property</span></span>|<span data-ttu-id="d747a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d747a-110">Type</span></span>|<span data-ttu-id="d747a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d747a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d747a-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d747a-112">userPrincipalName</span></span>|<span data-ttu-id="d747a-113">String</span><span class="sxs-lookup"><span data-stu-id="d747a-113">String</span></span>|<span data-ttu-id="d747a-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="d747a-114">User name</span></span>|
|<span data-ttu-id="d747a-115">дататосинк</span><span class="sxs-lookup"><span data-stu-id="d747a-115">dataToSync</span></span>|<span data-ttu-id="d747a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d747a-116">Boolean</span></span>|<span data-ttu-id="d747a-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="d747a-117">Data to sync</span></span>|
|<span data-ttu-id="d747a-118">Квота</span><span class="sxs-lookup"><span data-stu-id="d747a-118">dataQuota</span></span>|<span data-ttu-id="d747a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d747a-119">Int64</span></span>|<span data-ttu-id="d747a-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="d747a-120">Data quota</span></span>|
|<span data-ttu-id="d747a-121">Используется</span><span class="sxs-lookup"><span data-stu-id="d747a-121">dataUsed</span></span>|<span data-ttu-id="d747a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d747a-122">Int64</span></span>|<span data-ttu-id="d747a-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="d747a-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="d747a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="d747a-124">Relationships</span></span>
<span data-ttu-id="d747a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d747a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d747a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d747a-126">JSON Representation</span></span>
<span data-ttu-id="d747a-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d747a-127">Here is a JSON representation of the resource.</span></span>
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



