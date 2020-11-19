---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ada71a184dd0d7f25c774920b6f7d6b3da9fa438
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297723"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="d30e9-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="d30e9-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="d30e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d30e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d30e9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d30e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d30e9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d30e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d30e9-107">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="d30e9-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="d30e9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d30e9-108">Properties</span></span>
|<span data-ttu-id="d30e9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d30e9-109">Property</span></span>|<span data-ttu-id="d30e9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d30e9-110">Type</span></span>|<span data-ttu-id="d30e9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d30e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d30e9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d30e9-112">displayName</span></span>|<span data-ttu-id="d30e9-113">String</span><span class="sxs-lookup"><span data-stu-id="d30e9-113">String</span></span>|<span data-ttu-id="d30e9-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="d30e9-114">App display name.</span></span>|
|<span data-ttu-id="d30e9-115">description</span><span class="sxs-lookup"><span data-stu-id="d30e9-115">description</span></span>|<span data-ttu-id="d30e9-116">String</span><span class="sxs-lookup"><span data-stu-id="d30e9-116">String</span></span>|<span data-ttu-id="d30e9-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d30e9-117">The app's description.</span></span>|
|<span data-ttu-id="d30e9-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="d30e9-118">publisherName</span></span>|<span data-ttu-id="d30e9-119">String</span><span class="sxs-lookup"><span data-stu-id="d30e9-119">String</span></span>|<span data-ttu-id="d30e9-120">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="d30e9-120">The publisher name</span></span>|
|<span data-ttu-id="d30e9-121">productName</span><span class="sxs-lookup"><span data-stu-id="d30e9-121">productName</span></span>|<span data-ttu-id="d30e9-122">String</span><span class="sxs-lookup"><span data-stu-id="d30e9-122">String</span></span>|<span data-ttu-id="d30e9-123">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="d30e9-123">The product name.</span></span>|
|<span data-ttu-id="d30e9-124">denied</span><span class="sxs-lookup"><span data-stu-id="d30e9-124">denied</span></span>|<span data-ttu-id="d30e9-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="d30e9-125">Boolean</span></span>|<span data-ttu-id="d30e9-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="d30e9-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d30e9-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d30e9-127">Relationships</span></span>
<span data-ttu-id="d30e9-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d30e9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d30e9-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d30e9-129">JSON Representation</span></span>
<span data-ttu-id="d30e9-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d30e9-130">Here is a JSON representation of the resource.</span></span>
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




