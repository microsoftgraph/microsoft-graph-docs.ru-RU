---
title: Тип ресурса sharedAppleDeviceUser
description: Н/Д
ms.openlocfilehash: 79ebc5ae520c1c9b40bffb6a86e95693c52fa1e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076765"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="84631-103">Тип ресурса sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="84631-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="84631-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84631-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84631-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84631-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84631-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84631-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84631-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="84631-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="84631-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="84631-108">Properties</span></span>
|<span data-ttu-id="84631-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="84631-109">Property</span></span>|<span data-ttu-id="84631-110">Тип</span><span class="sxs-lookup"><span data-stu-id="84631-110">Type</span></span>|<span data-ttu-id="84631-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84631-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84631-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84631-112">userPrincipalName</span></span>|<span data-ttu-id="84631-113">String</span><span class="sxs-lookup"><span data-stu-id="84631-113">String</span></span>|<span data-ttu-id="84631-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="84631-114">User name</span></span>|
|<span data-ttu-id="84631-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="84631-115">dataToSync</span></span>|<span data-ttu-id="84631-116">Логический</span><span class="sxs-lookup"><span data-stu-id="84631-116">Boolean</span></span>|<span data-ttu-id="84631-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="84631-117">Data to sync</span></span>|
|<span data-ttu-id="84631-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="84631-118">dataQuota</span></span>|<span data-ttu-id="84631-119">Int64</span><span class="sxs-lookup"><span data-stu-id="84631-119">Int64</span></span>|<span data-ttu-id="84631-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="84631-120">Data quota</span></span>|
|<span data-ttu-id="84631-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="84631-121">dataUsed</span></span>|<span data-ttu-id="84631-122">Int64</span><span class="sxs-lookup"><span data-stu-id="84631-122">Int64</span></span>|<span data-ttu-id="84631-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="84631-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="84631-124">Связи</span><span class="sxs-lookup"><span data-stu-id="84631-124">Relationships</span></span>
<span data-ttu-id="84631-125">Нет</span><span class="sxs-lookup"><span data-stu-id="84631-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84631-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84631-126">JSON Representation</span></span>
<span data-ttu-id="84631-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84631-127">Here is a JSON representation of the resource.</span></span>
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





