---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6bc6b00185db677901e5e6a888e8b6b8197dfe1b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727283"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="60777-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="60777-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="60777-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60777-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60777-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60777-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60777-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60777-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60777-107">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="60777-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="60777-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="60777-108">Properties</span></span>
|<span data-ttu-id="60777-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="60777-109">Property</span></span>|<span data-ttu-id="60777-110">Тип</span><span class="sxs-lookup"><span data-stu-id="60777-110">Type</span></span>|<span data-ttu-id="60777-111">Описание</span><span class="sxs-lookup"><span data-stu-id="60777-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60777-112">displayName</span><span class="sxs-lookup"><span data-stu-id="60777-112">displayName</span></span>|<span data-ttu-id="60777-113">Строка</span><span class="sxs-lookup"><span data-stu-id="60777-113">String</span></span>|<span data-ttu-id="60777-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="60777-114">App display name.</span></span>|
|<span data-ttu-id="60777-115">description</span><span class="sxs-lookup"><span data-stu-id="60777-115">description</span></span>|<span data-ttu-id="60777-116">Строка</span><span class="sxs-lookup"><span data-stu-id="60777-116">String</span></span>|<span data-ttu-id="60777-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="60777-117">The app's description.</span></span>|
|<span data-ttu-id="60777-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="60777-118">publisherName</span></span>|<span data-ttu-id="60777-119">String</span><span class="sxs-lookup"><span data-stu-id="60777-119">String</span></span>|<span data-ttu-id="60777-120">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="60777-120">The publisher name</span></span>|
|<span data-ttu-id="60777-121">productName</span><span class="sxs-lookup"><span data-stu-id="60777-121">productName</span></span>|<span data-ttu-id="60777-122">String</span><span class="sxs-lookup"><span data-stu-id="60777-122">String</span></span>|<span data-ttu-id="60777-123">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="60777-123">The product name.</span></span>|
|<span data-ttu-id="60777-124">denied</span><span class="sxs-lookup"><span data-stu-id="60777-124">denied</span></span>|<span data-ttu-id="60777-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="60777-125">Boolean</span></span>|<span data-ttu-id="60777-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="60777-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60777-127">Связи</span><span class="sxs-lookup"><span data-stu-id="60777-127">Relationships</span></span>
<span data-ttu-id="60777-128">Нет</span><span class="sxs-lookup"><span data-stu-id="60777-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60777-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60777-129">JSON Representation</span></span>
<span data-ttu-id="60777-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60777-130">Here is a JSON representation of the resource.</span></span>
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





