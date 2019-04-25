---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb14092fa9f347e551a4871da69d9a3631b96e8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579179"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="8c632-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="8c632-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="8c632-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c632-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c632-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c632-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c632-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="8c632-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="8c632-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c632-107">Properties</span></span>
|<span data-ttu-id="8c632-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c632-108">Property</span></span>|<span data-ttu-id="8c632-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8c632-109">Type</span></span>|<span data-ttu-id="8c632-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c632-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c632-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8c632-111">displayName</span></span>|<span data-ttu-id="8c632-112">Строка</span><span class="sxs-lookup"><span data-stu-id="8c632-112">String</span></span>|<span data-ttu-id="8c632-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="8c632-113">App display name.</span></span>|
|<span data-ttu-id="8c632-114">description</span><span class="sxs-lookup"><span data-stu-id="8c632-114">description</span></span>|<span data-ttu-id="8c632-115">String</span><span class="sxs-lookup"><span data-stu-id="8c632-115">String</span></span>|<span data-ttu-id="8c632-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8c632-116">The app's description.</span></span>|
|<span data-ttu-id="8c632-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="8c632-117">publisherName</span></span>|<span data-ttu-id="8c632-118">String</span><span class="sxs-lookup"><span data-stu-id="8c632-118">String</span></span>|<span data-ttu-id="8c632-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="8c632-119">The publisher name</span></span>|
|<span data-ttu-id="8c632-120">productName</span><span class="sxs-lookup"><span data-stu-id="8c632-120">productName</span></span>|<span data-ttu-id="8c632-121">String</span><span class="sxs-lookup"><span data-stu-id="8c632-121">String</span></span>|<span data-ttu-id="8c632-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="8c632-122">The product name.</span></span>|
|<span data-ttu-id="8c632-123">denied</span><span class="sxs-lookup"><span data-stu-id="8c632-123">denied</span></span>|<span data-ttu-id="8c632-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c632-124">Boolean</span></span>|<span data-ttu-id="8c632-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="8c632-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c632-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="8c632-126">Relationships</span></span>
<span data-ttu-id="8c632-127">Нет</span><span class="sxs-lookup"><span data-stu-id="8c632-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c632-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c632-128">JSON Representation</span></span>
<span data-ttu-id="8c632-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c632-129">Here is a JSON representation of the resource.</span></span>
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





