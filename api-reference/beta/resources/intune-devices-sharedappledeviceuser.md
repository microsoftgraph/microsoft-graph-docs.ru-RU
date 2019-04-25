---
title: Тип ресурса Шаредаппледевицеусер
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43bc64243cb330f0761c8ded3ab646a0cde4f926
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526114"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="f6147-103">Тип ресурса Шаредаппледевицеусер</span><span class="sxs-lookup"><span data-stu-id="f6147-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="f6147-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6147-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6147-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6147-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6147-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f6147-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f6147-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6147-107">Properties</span></span>
|<span data-ttu-id="f6147-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6147-108">Property</span></span>|<span data-ttu-id="f6147-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f6147-109">Type</span></span>|<span data-ttu-id="f6147-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6147-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6147-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6147-111">userPrincipalName</span></span>|<span data-ttu-id="f6147-112">String</span><span class="sxs-lookup"><span data-stu-id="f6147-112">String</span></span>|<span data-ttu-id="f6147-113">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="f6147-113">User name</span></span>|
|<span data-ttu-id="f6147-114">Дататосинк</span><span class="sxs-lookup"><span data-stu-id="f6147-114">dataToSync</span></span>|<span data-ttu-id="f6147-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6147-115">Boolean</span></span>|<span data-ttu-id="f6147-116">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="f6147-116">Data to sync</span></span>|
|<span data-ttu-id="f6147-117">Квота</span><span class="sxs-lookup"><span data-stu-id="f6147-117">dataQuota</span></span>|<span data-ttu-id="f6147-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f6147-118">Int64</span></span>|<span data-ttu-id="f6147-119">Квота данных</span><span class="sxs-lookup"><span data-stu-id="f6147-119">Data quota</span></span>|
|<span data-ttu-id="f6147-120">Используется</span><span class="sxs-lookup"><span data-stu-id="f6147-120">dataUsed</span></span>|<span data-ttu-id="f6147-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f6147-121">Int64</span></span>|<span data-ttu-id="f6147-122">Квота данных</span><span class="sxs-lookup"><span data-stu-id="f6147-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6147-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="f6147-123">Relationships</span></span>
<span data-ttu-id="f6147-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f6147-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6147-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6147-125">JSON Representation</span></span>
<span data-ttu-id="f6147-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6147-126">Here is a JSON representation of the resource.</span></span>
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





