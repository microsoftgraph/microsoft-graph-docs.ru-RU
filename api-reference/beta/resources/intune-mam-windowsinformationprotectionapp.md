---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4b5858a09a775b28d12c258bcdca82dc302f813
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994540"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="f0c96-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="f0c96-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="f0c96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0c96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0c96-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0c96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0c96-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="f0c96-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="f0c96-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0c96-107">Properties</span></span>
|<span data-ttu-id="f0c96-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0c96-108">Property</span></span>|<span data-ttu-id="f0c96-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f0c96-109">Type</span></span>|<span data-ttu-id="f0c96-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f0c96-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0c96-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f0c96-111">displayName</span></span>|<span data-ttu-id="f0c96-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f0c96-112">String</span></span>|<span data-ttu-id="f0c96-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="f0c96-113">App display name.</span></span>|
|<span data-ttu-id="f0c96-114">description</span><span class="sxs-lookup"><span data-stu-id="f0c96-114">description</span></span>|<span data-ttu-id="f0c96-115">Строка</span><span class="sxs-lookup"><span data-stu-id="f0c96-115">String</span></span>|<span data-ttu-id="f0c96-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f0c96-116">The app's description.</span></span>|
|<span data-ttu-id="f0c96-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="f0c96-117">publisherName</span></span>|<span data-ttu-id="f0c96-118">String</span><span class="sxs-lookup"><span data-stu-id="f0c96-118">String</span></span>|<span data-ttu-id="f0c96-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="f0c96-119">The publisher name</span></span>|
|<span data-ttu-id="f0c96-120">productName</span><span class="sxs-lookup"><span data-stu-id="f0c96-120">productName</span></span>|<span data-ttu-id="f0c96-121">String</span><span class="sxs-lookup"><span data-stu-id="f0c96-121">String</span></span>|<span data-ttu-id="f0c96-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="f0c96-122">The product name.</span></span>|
|<span data-ttu-id="f0c96-123">denied</span><span class="sxs-lookup"><span data-stu-id="f0c96-123">denied</span></span>|<span data-ttu-id="f0c96-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0c96-124">Boolean</span></span>|<span data-ttu-id="f0c96-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="f0c96-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0c96-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="f0c96-126">Relationships</span></span>
<span data-ttu-id="f0c96-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f0c96-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0c96-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0c96-128">JSON Representation</span></span>
<span data-ttu-id="f0c96-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0c96-129">Here is a JSON representation of the resource.</span></span>
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





