---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03dd609b8bd2c1835665827fff2bd89f6e810d77
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751295"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="4fe76-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="4fe76-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="4fe76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fe76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fe76-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fe76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fe76-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="4fe76-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="4fe76-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fe76-107">Properties</span></span>
|<span data-ttu-id="4fe76-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fe76-108">Property</span></span>|<span data-ttu-id="4fe76-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4fe76-109">Type</span></span>|<span data-ttu-id="4fe76-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4fe76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fe76-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4fe76-111">displayName</span></span>|<span data-ttu-id="4fe76-112">String</span><span class="sxs-lookup"><span data-stu-id="4fe76-112">String</span></span>|<span data-ttu-id="4fe76-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="4fe76-113">App display name.</span></span>|
|<span data-ttu-id="4fe76-114">description</span><span class="sxs-lookup"><span data-stu-id="4fe76-114">description</span></span>|<span data-ttu-id="4fe76-115">String</span><span class="sxs-lookup"><span data-stu-id="4fe76-115">String</span></span>|<span data-ttu-id="4fe76-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4fe76-116">The app's description.</span></span>|
|<span data-ttu-id="4fe76-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="4fe76-117">publisherName</span></span>|<span data-ttu-id="4fe76-118">String</span><span class="sxs-lookup"><span data-stu-id="4fe76-118">String</span></span>|<span data-ttu-id="4fe76-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="4fe76-119">The publisher name</span></span>|
|<span data-ttu-id="4fe76-120">productName</span><span class="sxs-lookup"><span data-stu-id="4fe76-120">productName</span></span>|<span data-ttu-id="4fe76-121">String</span><span class="sxs-lookup"><span data-stu-id="4fe76-121">String</span></span>|<span data-ttu-id="4fe76-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="4fe76-122">The product name.</span></span>|
|<span data-ttu-id="4fe76-123">denied</span><span class="sxs-lookup"><span data-stu-id="4fe76-123">denied</span></span>|<span data-ttu-id="4fe76-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fe76-124">Boolean</span></span>|<span data-ttu-id="4fe76-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="4fe76-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fe76-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="4fe76-126">Relationships</span></span>
<span data-ttu-id="4fe76-127">Нет</span><span class="sxs-lookup"><span data-stu-id="4fe76-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fe76-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fe76-128">JSON Representation</span></span>
<span data-ttu-id="4fe76-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fe76-129">Here is a JSON representation of the resource.</span></span>
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




