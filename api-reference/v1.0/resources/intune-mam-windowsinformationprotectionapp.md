---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d025b20e5341c17f756e86bb6bb84faf92a61a3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971881"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="212fb-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="212fb-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="212fb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="212fb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="212fb-105">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="212fb-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="212fb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="212fb-106">Properties</span></span>
|<span data-ttu-id="212fb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="212fb-107">Property</span></span>|<span data-ttu-id="212fb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="212fb-108">Type</span></span>|<span data-ttu-id="212fb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="212fb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="212fb-110">displayName</span><span class="sxs-lookup"><span data-stu-id="212fb-110">displayName</span></span>|<span data-ttu-id="212fb-111">String</span><span class="sxs-lookup"><span data-stu-id="212fb-111">String</span></span>|<span data-ttu-id="212fb-112">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="212fb-112">App display name.</span></span>|
|<span data-ttu-id="212fb-113">описание</span><span class="sxs-lookup"><span data-stu-id="212fb-113">description</span></span>|<span data-ttu-id="212fb-114">String</span><span class="sxs-lookup"><span data-stu-id="212fb-114">String</span></span>|<span data-ttu-id="212fb-115">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="212fb-115">The app's description.</span></span>|
|<span data-ttu-id="212fb-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="212fb-116">publisherName</span></span>|<span data-ttu-id="212fb-117">String</span><span class="sxs-lookup"><span data-stu-id="212fb-117">String</span></span>|<span data-ttu-id="212fb-118">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="212fb-118">The publisher name</span></span>|
|<span data-ttu-id="212fb-119">productName</span><span class="sxs-lookup"><span data-stu-id="212fb-119">productName</span></span>|<span data-ttu-id="212fb-120">String</span><span class="sxs-lookup"><span data-stu-id="212fb-120">String</span></span>|<span data-ttu-id="212fb-121">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="212fb-121">The product name.</span></span>|
|<span data-ttu-id="212fb-122">denied</span><span class="sxs-lookup"><span data-stu-id="212fb-122">denied</span></span>|<span data-ttu-id="212fb-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="212fb-123">Boolean</span></span>|<span data-ttu-id="212fb-124">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="212fb-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="212fb-125">Связи</span><span class="sxs-lookup"><span data-stu-id="212fb-125">Relationships</span></span>
<span data-ttu-id="212fb-126">Нет</span><span class="sxs-lookup"><span data-stu-id="212fb-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="212fb-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="212fb-127">JSON Representation</span></span>
<span data-ttu-id="212fb-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="212fb-128">Here is a JSON representation of the resource.</span></span>
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



