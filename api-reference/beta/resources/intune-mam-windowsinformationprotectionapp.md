---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e7cd7225783edd3e2e86d4d60ea2705568245d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524275"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="00e7b-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="00e7b-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="00e7b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00e7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00e7b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00e7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00e7b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00e7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00e7b-107">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="00e7b-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="00e7b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="00e7b-108">Properties</span></span>
|<span data-ttu-id="00e7b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="00e7b-109">Property</span></span>|<span data-ttu-id="00e7b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="00e7b-110">Type</span></span>|<span data-ttu-id="00e7b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="00e7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00e7b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="00e7b-112">displayName</span></span>|<span data-ttu-id="00e7b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="00e7b-113">String</span></span>|<span data-ttu-id="00e7b-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="00e7b-114">App display name.</span></span>|
|<span data-ttu-id="00e7b-115">description</span><span class="sxs-lookup"><span data-stu-id="00e7b-115">description</span></span>|<span data-ttu-id="00e7b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="00e7b-116">String</span></span>|<span data-ttu-id="00e7b-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="00e7b-117">The app's description.</span></span>|
|<span data-ttu-id="00e7b-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="00e7b-118">publisherName</span></span>|<span data-ttu-id="00e7b-119">String</span><span class="sxs-lookup"><span data-stu-id="00e7b-119">String</span></span>|<span data-ttu-id="00e7b-120">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="00e7b-120">The publisher name</span></span>|
|<span data-ttu-id="00e7b-121">productName</span><span class="sxs-lookup"><span data-stu-id="00e7b-121">productName</span></span>|<span data-ttu-id="00e7b-122">String</span><span class="sxs-lookup"><span data-stu-id="00e7b-122">String</span></span>|<span data-ttu-id="00e7b-123">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="00e7b-123">The product name.</span></span>|
|<span data-ttu-id="00e7b-124">denied</span><span class="sxs-lookup"><span data-stu-id="00e7b-124">denied</span></span>|<span data-ttu-id="00e7b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="00e7b-125">Boolean</span></span>|<span data-ttu-id="00e7b-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="00e7b-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00e7b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="00e7b-127">Relationships</span></span>
<span data-ttu-id="00e7b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="00e7b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00e7b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00e7b-129">JSON Representation</span></span>
<span data-ttu-id="00e7b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00e7b-130">Here is a JSON representation of the resource.</span></span>
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



