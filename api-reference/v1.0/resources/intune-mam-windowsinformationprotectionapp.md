---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
ms.openlocfilehash: 0ea48e087d4a8450ee47b2239b7c67f3b050da85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025071"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="2ae4f-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="2ae4f-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="2ae4f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2ae4f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ae4f-105">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="2ae4f-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="2ae4f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ae4f-106">Properties</span></span>
|<span data-ttu-id="2ae4f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ae4f-107">Property</span></span>|<span data-ttu-id="2ae4f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2ae4f-108">Type</span></span>|<span data-ttu-id="2ae4f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2ae4f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ae4f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="2ae4f-110">displayName</span></span>|<span data-ttu-id="2ae4f-111">String</span><span class="sxs-lookup"><span data-stu-id="2ae4f-111">String</span></span>|<span data-ttu-id="2ae4f-112">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="2ae4f-112">App display name.</span></span>|
|<span data-ttu-id="2ae4f-113">описание</span><span class="sxs-lookup"><span data-stu-id="2ae4f-113">description</span></span>|<span data-ttu-id="2ae4f-114">String</span><span class="sxs-lookup"><span data-stu-id="2ae4f-114">String</span></span>|<span data-ttu-id="2ae4f-115">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2ae4f-115">The app's description.</span></span>|
|<span data-ttu-id="2ae4f-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="2ae4f-116">publisherName</span></span>|<span data-ttu-id="2ae4f-117">String</span><span class="sxs-lookup"><span data-stu-id="2ae4f-117">String</span></span>|<span data-ttu-id="2ae4f-118">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="2ae4f-118">The publisher name</span></span>|
|<span data-ttu-id="2ae4f-119">productName</span><span class="sxs-lookup"><span data-stu-id="2ae4f-119">productName</span></span>|<span data-ttu-id="2ae4f-120">String</span><span class="sxs-lookup"><span data-stu-id="2ae4f-120">String</span></span>|<span data-ttu-id="2ae4f-121">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="2ae4f-121">The product name.</span></span>|
|<span data-ttu-id="2ae4f-122">denied</span><span class="sxs-lookup"><span data-stu-id="2ae4f-122">denied</span></span>|<span data-ttu-id="2ae4f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ae4f-123">Boolean</span></span>|<span data-ttu-id="2ae4f-124">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="2ae4f-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ae4f-125">Связи</span><span class="sxs-lookup"><span data-stu-id="2ae4f-125">Relationships</span></span>
<span data-ttu-id="2ae4f-126">Нет</span><span class="sxs-lookup"><span data-stu-id="2ae4f-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ae4f-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ae4f-127">JSON Representation</span></span>
<span data-ttu-id="2ae4f-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ae4f-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



