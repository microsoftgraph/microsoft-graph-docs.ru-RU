---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08a1ed7d56c41eee69ee907a9efd91c12fad9b4e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373261"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="534e2-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="534e2-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="534e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="534e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="534e2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="534e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="534e2-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="534e2-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="534e2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="534e2-107">Properties</span></span>
|<span data-ttu-id="534e2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="534e2-108">Property</span></span>|<span data-ttu-id="534e2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="534e2-109">Type</span></span>|<span data-ttu-id="534e2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="534e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="534e2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="534e2-111">displayName</span></span>|<span data-ttu-id="534e2-112">Строка</span><span class="sxs-lookup"><span data-stu-id="534e2-112">String</span></span>|<span data-ttu-id="534e2-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="534e2-113">App display name.</span></span>|
|<span data-ttu-id="534e2-114">description</span><span class="sxs-lookup"><span data-stu-id="534e2-114">description</span></span>|<span data-ttu-id="534e2-115">Строка</span><span class="sxs-lookup"><span data-stu-id="534e2-115">String</span></span>|<span data-ttu-id="534e2-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="534e2-116">The app's description.</span></span>|
|<span data-ttu-id="534e2-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="534e2-117">publisherName</span></span>|<span data-ttu-id="534e2-118">String</span><span class="sxs-lookup"><span data-stu-id="534e2-118">String</span></span>|<span data-ttu-id="534e2-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="534e2-119">The publisher name</span></span>|
|<span data-ttu-id="534e2-120">productName</span><span class="sxs-lookup"><span data-stu-id="534e2-120">productName</span></span>|<span data-ttu-id="534e2-121">String</span><span class="sxs-lookup"><span data-stu-id="534e2-121">String</span></span>|<span data-ttu-id="534e2-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="534e2-122">The product name.</span></span>|
|<span data-ttu-id="534e2-123">denied</span><span class="sxs-lookup"><span data-stu-id="534e2-123">denied</span></span>|<span data-ttu-id="534e2-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="534e2-124">Boolean</span></span>|<span data-ttu-id="534e2-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="534e2-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="534e2-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="534e2-126">Relationships</span></span>
<span data-ttu-id="534e2-127">Нет</span><span class="sxs-lookup"><span data-stu-id="534e2-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="534e2-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="534e2-128">JSON Representation</span></span>
<span data-ttu-id="534e2-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="534e2-129">Here is a JSON representation of the resource.</span></span>
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



