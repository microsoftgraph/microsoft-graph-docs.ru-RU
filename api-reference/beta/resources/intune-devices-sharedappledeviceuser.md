---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87ea9c12632fd1bb6fc7df17cd7f732560eedb8f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993938"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="c3a43-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="c3a43-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="c3a43-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3a43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3a43-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3a43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a43-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c3a43-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c3a43-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3a43-107">Properties</span></span>
|<span data-ttu-id="c3a43-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3a43-108">Property</span></span>|<span data-ttu-id="c3a43-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c3a43-109">Type</span></span>|<span data-ttu-id="c3a43-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c3a43-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a43-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c3a43-111">userPrincipalName</span></span>|<span data-ttu-id="c3a43-112">String</span><span class="sxs-lookup"><span data-stu-id="c3a43-112">String</span></span>|<span data-ttu-id="c3a43-113">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="c3a43-113">User name</span></span>|
|<span data-ttu-id="c3a43-114">Дататосинк</span><span class="sxs-lookup"><span data-stu-id="c3a43-114">dataToSync</span></span>|<span data-ttu-id="c3a43-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3a43-115">Boolean</span></span>|<span data-ttu-id="c3a43-116">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="c3a43-116">Data to sync</span></span>|
|<span data-ttu-id="c3a43-117">Квота</span><span class="sxs-lookup"><span data-stu-id="c3a43-117">dataQuota</span></span>|<span data-ttu-id="c3a43-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c3a43-118">Int64</span></span>|<span data-ttu-id="c3a43-119">Квота данных</span><span class="sxs-lookup"><span data-stu-id="c3a43-119">Data quota</span></span>|
|<span data-ttu-id="c3a43-120">Используется</span><span class="sxs-lookup"><span data-stu-id="c3a43-120">dataUsed</span></span>|<span data-ttu-id="c3a43-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c3a43-121">Int64</span></span>|<span data-ttu-id="c3a43-122">Квота данных</span><span class="sxs-lookup"><span data-stu-id="c3a43-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3a43-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="c3a43-123">Relationships</span></span>
<span data-ttu-id="c3a43-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c3a43-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3a43-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3a43-125">JSON Representation</span></span>
<span data-ttu-id="c3a43-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3a43-126">Here is a JSON representation of the resource.</span></span>
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





