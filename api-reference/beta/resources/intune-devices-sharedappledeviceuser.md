---
title: Тип ресурса sharedAppleDeviceUser
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5ee74080b95328cf55813dc628ee7a517dff08e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806855"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="b5477-103">Тип ресурса sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="b5477-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="b5477-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b5477-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5477-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5477-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5477-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b5477-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5477-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b5477-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b5477-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5477-108">Properties</span></span>
|<span data-ttu-id="b5477-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5477-109">Property</span></span>|<span data-ttu-id="b5477-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b5477-110">Type</span></span>|<span data-ttu-id="b5477-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b5477-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5477-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b5477-112">userPrincipalName</span></span>|<span data-ttu-id="b5477-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b5477-113">String</span></span>|<span data-ttu-id="b5477-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="b5477-114">User name</span></span>|
|<span data-ttu-id="b5477-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="b5477-115">dataToSync</span></span>|<span data-ttu-id="b5477-116">Логический</span><span class="sxs-lookup"><span data-stu-id="b5477-116">Boolean</span></span>|<span data-ttu-id="b5477-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="b5477-117">Data to sync</span></span>|
|<span data-ttu-id="b5477-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="b5477-118">dataQuota</span></span>|<span data-ttu-id="b5477-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b5477-119">Int64</span></span>|<span data-ttu-id="b5477-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="b5477-120">Data quota</span></span>|
|<span data-ttu-id="b5477-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="b5477-121">dataUsed</span></span>|<span data-ttu-id="b5477-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b5477-122">Int64</span></span>|<span data-ttu-id="b5477-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="b5477-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5477-124">Связи</span><span class="sxs-lookup"><span data-stu-id="b5477-124">Relationships</span></span>
<span data-ttu-id="b5477-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b5477-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5477-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5477-126">JSON Representation</span></span>
<span data-ttu-id="b5477-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5477-127">Here is a JSON representation of the resource.</span></span>
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





