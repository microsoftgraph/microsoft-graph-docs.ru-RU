---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72b7654712241549aaa1377e48dfdc856dd3bc1b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940612"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="8c6ce-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="8c6ce-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="8c6ce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c6ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c6ce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c6ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c6ce-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="8c6ce-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="8c6ce-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c6ce-107">Properties</span></span>
|<span data-ttu-id="8c6ce-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c6ce-108">Property</span></span>|<span data-ttu-id="8c6ce-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8c6ce-109">Type</span></span>|<span data-ttu-id="8c6ce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c6ce-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c6ce-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8c6ce-111">displayName</span></span>|<span data-ttu-id="8c6ce-112">Строка</span><span class="sxs-lookup"><span data-stu-id="8c6ce-112">String</span></span>|<span data-ttu-id="8c6ce-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="8c6ce-113">App display name.</span></span>|
|<span data-ttu-id="8c6ce-114">description</span><span class="sxs-lookup"><span data-stu-id="8c6ce-114">description</span></span>|<span data-ttu-id="8c6ce-115">Строка</span><span class="sxs-lookup"><span data-stu-id="8c6ce-115">String</span></span>|<span data-ttu-id="8c6ce-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8c6ce-116">The app's description.</span></span>|
|<span data-ttu-id="8c6ce-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="8c6ce-117">publisherName</span></span>|<span data-ttu-id="8c6ce-118">String</span><span class="sxs-lookup"><span data-stu-id="8c6ce-118">String</span></span>|<span data-ttu-id="8c6ce-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="8c6ce-119">The publisher name</span></span>|
|<span data-ttu-id="8c6ce-120">productName</span><span class="sxs-lookup"><span data-stu-id="8c6ce-120">productName</span></span>|<span data-ttu-id="8c6ce-121">String</span><span class="sxs-lookup"><span data-stu-id="8c6ce-121">String</span></span>|<span data-ttu-id="8c6ce-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="8c6ce-122">The product name.</span></span>|
|<span data-ttu-id="8c6ce-123">denied</span><span class="sxs-lookup"><span data-stu-id="8c6ce-123">denied</span></span>|<span data-ttu-id="8c6ce-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c6ce-124">Boolean</span></span>|<span data-ttu-id="8c6ce-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="8c6ce-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c6ce-126">Связи</span><span class="sxs-lookup"><span data-stu-id="8c6ce-126">Relationships</span></span>
<span data-ttu-id="8c6ce-127">Нет</span><span class="sxs-lookup"><span data-stu-id="8c6ce-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c6ce-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c6ce-128">JSON Representation</span></span>
<span data-ttu-id="8c6ce-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c6ce-129">Here is a JSON representation of the resource.</span></span>
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




