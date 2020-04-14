---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b255fdc604c5b1aacc4c7cbfd5750b01675fe335
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443762"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="4baf3-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="4baf3-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="4baf3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4baf3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4baf3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4baf3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4baf3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4baf3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4baf3-107">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="4baf3-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="4baf3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4baf3-108">Properties</span></span>
|<span data-ttu-id="4baf3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4baf3-109">Property</span></span>|<span data-ttu-id="4baf3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4baf3-110">Type</span></span>|<span data-ttu-id="4baf3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4baf3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4baf3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4baf3-112">displayName</span></span>|<span data-ttu-id="4baf3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="4baf3-113">String</span></span>|<span data-ttu-id="4baf3-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="4baf3-114">App display name.</span></span>|
|<span data-ttu-id="4baf3-115">description</span><span class="sxs-lookup"><span data-stu-id="4baf3-115">description</span></span>|<span data-ttu-id="4baf3-116">Строка</span><span class="sxs-lookup"><span data-stu-id="4baf3-116">String</span></span>|<span data-ttu-id="4baf3-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4baf3-117">The app's description.</span></span>|
|<span data-ttu-id="4baf3-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="4baf3-118">publisherName</span></span>|<span data-ttu-id="4baf3-119">String</span><span class="sxs-lookup"><span data-stu-id="4baf3-119">String</span></span>|<span data-ttu-id="4baf3-120">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="4baf3-120">The publisher name</span></span>|
|<span data-ttu-id="4baf3-121">productName</span><span class="sxs-lookup"><span data-stu-id="4baf3-121">productName</span></span>|<span data-ttu-id="4baf3-122">String</span><span class="sxs-lookup"><span data-stu-id="4baf3-122">String</span></span>|<span data-ttu-id="4baf3-123">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="4baf3-123">The product name.</span></span>|
|<span data-ttu-id="4baf3-124">denied</span><span class="sxs-lookup"><span data-stu-id="4baf3-124">denied</span></span>|<span data-ttu-id="4baf3-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4baf3-125">Boolean</span></span>|<span data-ttu-id="4baf3-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="4baf3-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4baf3-127">Связи</span><span class="sxs-lookup"><span data-stu-id="4baf3-127">Relationships</span></span>
<span data-ttu-id="4baf3-128">Нет</span><span class="sxs-lookup"><span data-stu-id="4baf3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4baf3-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4baf3-129">JSON Representation</span></span>
<span data-ttu-id="4baf3-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4baf3-130">Here is a JSON representation of the resource.</span></span>
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



