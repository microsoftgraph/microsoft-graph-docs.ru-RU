---
title: Тип ресурса sharedAppleDeviceUser
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6106daff0b7c4af023c8bfbb8352b52efc674928
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987708"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="94e18-103">Тип ресурса sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="94e18-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="94e18-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="94e18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94e18-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94e18-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="94e18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94e18-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="94e18-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="94e18-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="94e18-108">Properties</span></span>
|<span data-ttu-id="94e18-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="94e18-109">Property</span></span>|<span data-ttu-id="94e18-110">Тип</span><span class="sxs-lookup"><span data-stu-id="94e18-110">Type</span></span>|<span data-ttu-id="94e18-111">Описание</span><span class="sxs-lookup"><span data-stu-id="94e18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94e18-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="94e18-112">userPrincipalName</span></span>|<span data-ttu-id="94e18-113">Строка</span><span class="sxs-lookup"><span data-stu-id="94e18-113">String</span></span>|<span data-ttu-id="94e18-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="94e18-114">User name</span></span>|
|<span data-ttu-id="94e18-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="94e18-115">dataToSync</span></span>|<span data-ttu-id="94e18-116">Логический</span><span class="sxs-lookup"><span data-stu-id="94e18-116">Boolean</span></span>|<span data-ttu-id="94e18-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="94e18-117">Data to sync</span></span>|
|<span data-ttu-id="94e18-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="94e18-118">dataQuota</span></span>|<span data-ttu-id="94e18-119">Int64</span><span class="sxs-lookup"><span data-stu-id="94e18-119">Int64</span></span>|<span data-ttu-id="94e18-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="94e18-120">Data quota</span></span>|
|<span data-ttu-id="94e18-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="94e18-121">dataUsed</span></span>|<span data-ttu-id="94e18-122">Int64</span><span class="sxs-lookup"><span data-stu-id="94e18-122">Int64</span></span>|<span data-ttu-id="94e18-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="94e18-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="94e18-124">Связи</span><span class="sxs-lookup"><span data-stu-id="94e18-124">Relationships</span></span>
<span data-ttu-id="94e18-125">Нет</span><span class="sxs-lookup"><span data-stu-id="94e18-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="94e18-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94e18-126">JSON Representation</span></span>
<span data-ttu-id="94e18-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94e18-127">Here is a JSON representation of the resource.</span></span>
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





