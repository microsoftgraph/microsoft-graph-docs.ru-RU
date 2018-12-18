---
title: Тип ресурса sharedAppleDeviceUser
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 4e16d691ed6286fb8046c0693292012e1e94a0ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315992"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="f9e0d-103">Тип ресурса sharedAppleDeviceUser</span><span class="sxs-lookup"><span data-stu-id="f9e0d-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="f9e0d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9e0d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9e0d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9e0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9e0d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f9e0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9e0d-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f9e0d-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f9e0d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9e0d-108">Properties</span></span>
|<span data-ttu-id="f9e0d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9e0d-109">Property</span></span>|<span data-ttu-id="f9e0d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9e0d-110">Type</span></span>|<span data-ttu-id="f9e0d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9e0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9e0d-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9e0d-112">userPrincipalName</span></span>|<span data-ttu-id="f9e0d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f9e0d-113">String</span></span>|<span data-ttu-id="f9e0d-114">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="f9e0d-114">User name</span></span>|
|<span data-ttu-id="f9e0d-115">dataToSync</span><span class="sxs-lookup"><span data-stu-id="f9e0d-115">dataToSync</span></span>|<span data-ttu-id="f9e0d-116">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f9e0d-116">Boolean</span></span>|<span data-ttu-id="f9e0d-117">Данные для синхронизации</span><span class="sxs-lookup"><span data-stu-id="f9e0d-117">Data to sync</span></span>|
|<span data-ttu-id="f9e0d-118">dataQuota</span><span class="sxs-lookup"><span data-stu-id="f9e0d-118">dataQuota</span></span>|<span data-ttu-id="f9e0d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f9e0d-119">Int64</span></span>|<span data-ttu-id="f9e0d-120">Квота данных</span><span class="sxs-lookup"><span data-stu-id="f9e0d-120">Data quota</span></span>|
|<span data-ttu-id="f9e0d-121">dataUsed</span><span class="sxs-lookup"><span data-stu-id="f9e0d-121">dataUsed</span></span>|<span data-ttu-id="f9e0d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f9e0d-122">Int64</span></span>|<span data-ttu-id="f9e0d-123">Квота данных</span><span class="sxs-lookup"><span data-stu-id="f9e0d-123">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9e0d-124">Связи</span><span class="sxs-lookup"><span data-stu-id="f9e0d-124">Relationships</span></span>
<span data-ttu-id="f9e0d-125">Нет</span><span class="sxs-lookup"><span data-stu-id="f9e0d-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9e0d-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9e0d-126">JSON Representation</span></span>
<span data-ttu-id="f9e0d-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9e0d-127">Here is a JSON representation of the resource.</span></span>
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





