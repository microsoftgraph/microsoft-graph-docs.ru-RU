---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fbaa627cd8665678de148f8338a8570f57a2cb01
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780971"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="2d6de-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="2d6de-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="2d6de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d6de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d6de-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d6de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d6de-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="2d6de-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="2d6de-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d6de-107">Properties</span></span>
|<span data-ttu-id="2d6de-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d6de-108">Property</span></span>|<span data-ttu-id="2d6de-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2d6de-109">Type</span></span>|<span data-ttu-id="2d6de-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2d6de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d6de-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2d6de-111">displayName</span></span>|<span data-ttu-id="2d6de-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2d6de-112">String</span></span>|<span data-ttu-id="2d6de-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="2d6de-113">App display name.</span></span>|
|<span data-ttu-id="2d6de-114">description</span><span class="sxs-lookup"><span data-stu-id="2d6de-114">description</span></span>|<span data-ttu-id="2d6de-115">Строка</span><span class="sxs-lookup"><span data-stu-id="2d6de-115">String</span></span>|<span data-ttu-id="2d6de-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2d6de-116">The app's description.</span></span>|
|<span data-ttu-id="2d6de-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="2d6de-117">publisherName</span></span>|<span data-ttu-id="2d6de-118">String</span><span class="sxs-lookup"><span data-stu-id="2d6de-118">String</span></span>|<span data-ttu-id="2d6de-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="2d6de-119">The publisher name</span></span>|
|<span data-ttu-id="2d6de-120">productName</span><span class="sxs-lookup"><span data-stu-id="2d6de-120">productName</span></span>|<span data-ttu-id="2d6de-121">String</span><span class="sxs-lookup"><span data-stu-id="2d6de-121">String</span></span>|<span data-ttu-id="2d6de-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="2d6de-122">The product name.</span></span>|
|<span data-ttu-id="2d6de-123">denied</span><span class="sxs-lookup"><span data-stu-id="2d6de-123">denied</span></span>|<span data-ttu-id="2d6de-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d6de-124">Boolean</span></span>|<span data-ttu-id="2d6de-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="2d6de-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d6de-126">Связи</span><span class="sxs-lookup"><span data-stu-id="2d6de-126">Relationships</span></span>
<span data-ttu-id="2d6de-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2d6de-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d6de-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d6de-128">JSON Representation</span></span>
<span data-ttu-id="2d6de-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d6de-129">Here is a JSON representation of the resource.</span></span>
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



