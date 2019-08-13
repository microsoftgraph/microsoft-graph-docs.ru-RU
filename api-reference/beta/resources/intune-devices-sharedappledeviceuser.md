---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f71e4c6340b7dcf859e71cdf829b257794f443a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372638"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="f26f8-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="f26f8-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="f26f8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f26f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f26f8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f26f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f26f8-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f26f8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f26f8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f26f8-107">Properties</span></span>
|<span data-ttu-id="f26f8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f26f8-108">Property</span></span>|<span data-ttu-id="f26f8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f26f8-109">Type</span></span>|<span data-ttu-id="f26f8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f26f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f26f8-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f26f8-111">userPrincipalName</span></span>|<span data-ttu-id="f26f8-112">String</span><span class="sxs-lookup"><span data-stu-id="f26f8-112">String</span></span>|<span data-ttu-id="f26f8-113">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="f26f8-113">User name</span></span>|
|<span data-ttu-id="f26f8-114">дататосинк</span><span class="sxs-lookup"><span data-stu-id="f26f8-114">dataToSync</span></span>|<span data-ttu-id="f26f8-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f26f8-115">Boolean</span></span>|<span data-ttu-id="f26f8-116">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="f26f8-116">Data to sync</span></span>|
|<span data-ttu-id="f26f8-117">Квота</span><span class="sxs-lookup"><span data-stu-id="f26f8-117">dataQuota</span></span>|<span data-ttu-id="f26f8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f26f8-118">Int64</span></span>|<span data-ttu-id="f26f8-119">Квота данных</span><span class="sxs-lookup"><span data-stu-id="f26f8-119">Data quota</span></span>|
|<span data-ttu-id="f26f8-120">Используется</span><span class="sxs-lookup"><span data-stu-id="f26f8-120">dataUsed</span></span>|<span data-ttu-id="f26f8-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f26f8-121">Int64</span></span>|<span data-ttu-id="f26f8-122">Квота данных</span><span class="sxs-lookup"><span data-stu-id="f26f8-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="f26f8-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="f26f8-123">Relationships</span></span>
<span data-ttu-id="f26f8-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f26f8-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f26f8-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f26f8-125">JSON Representation</span></span>
<span data-ttu-id="f26f8-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f26f8-126">Here is a JSON representation of the resource.</span></span>
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



