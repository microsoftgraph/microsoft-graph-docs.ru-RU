---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59360d948865e184abab7b9749c764a43b2710d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030061"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="88806-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="88806-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="88806-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88806-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88806-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88806-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88806-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88806-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88806-107">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="88806-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="88806-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="88806-108">Properties</span></span>
|<span data-ttu-id="88806-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="88806-109">Property</span></span>|<span data-ttu-id="88806-110">Тип</span><span class="sxs-lookup"><span data-stu-id="88806-110">Type</span></span>|<span data-ttu-id="88806-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88806-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88806-112">displayName</span><span class="sxs-lookup"><span data-stu-id="88806-112">displayName</span></span>|<span data-ttu-id="88806-113">String</span><span class="sxs-lookup"><span data-stu-id="88806-113">String</span></span>|<span data-ttu-id="88806-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="88806-114">App display name.</span></span>|
|<span data-ttu-id="88806-115">description</span><span class="sxs-lookup"><span data-stu-id="88806-115">description</span></span>|<span data-ttu-id="88806-116">String</span><span class="sxs-lookup"><span data-stu-id="88806-116">String</span></span>|<span data-ttu-id="88806-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="88806-117">The app's description.</span></span>|
|<span data-ttu-id="88806-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="88806-118">publisherName</span></span>|<span data-ttu-id="88806-119">String</span><span class="sxs-lookup"><span data-stu-id="88806-119">String</span></span>|<span data-ttu-id="88806-120">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="88806-120">The publisher name</span></span>|
|<span data-ttu-id="88806-121">productName</span><span class="sxs-lookup"><span data-stu-id="88806-121">productName</span></span>|<span data-ttu-id="88806-122">String</span><span class="sxs-lookup"><span data-stu-id="88806-122">String</span></span>|<span data-ttu-id="88806-123">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="88806-123">The product name.</span></span>|
|<span data-ttu-id="88806-124">denied</span><span class="sxs-lookup"><span data-stu-id="88806-124">denied</span></span>|<span data-ttu-id="88806-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="88806-125">Boolean</span></span>|<span data-ttu-id="88806-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="88806-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88806-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="88806-127">Relationships</span></span>
<span data-ttu-id="88806-128">Нет</span><span class="sxs-lookup"><span data-stu-id="88806-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88806-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88806-129">JSON Representation</span></span>
<span data-ttu-id="88806-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88806-130">Here is a JSON representation of the resource.</span></span>
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






