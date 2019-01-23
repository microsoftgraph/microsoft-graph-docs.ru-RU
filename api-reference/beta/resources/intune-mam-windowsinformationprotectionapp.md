---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45d428ee18e92e76f5a13c568373219f904fd886
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403688"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="d3106-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="d3106-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="d3106-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d3106-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d3106-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3106-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3106-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3106-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3106-107">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="d3106-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="d3106-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3106-108">Properties</span></span>
|<span data-ttu-id="d3106-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3106-109">Property</span></span>|<span data-ttu-id="d3106-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d3106-110">Type</span></span>|<span data-ttu-id="d3106-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d3106-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3106-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d3106-112">displayName</span></span>|<span data-ttu-id="d3106-113">String</span><span class="sxs-lookup"><span data-stu-id="d3106-113">String</span></span>|<span data-ttu-id="d3106-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="d3106-114">App display name.</span></span>|
|<span data-ttu-id="d3106-115">description</span><span class="sxs-lookup"><span data-stu-id="d3106-115">description</span></span>|<span data-ttu-id="d3106-116">String</span><span class="sxs-lookup"><span data-stu-id="d3106-116">String</span></span>|<span data-ttu-id="d3106-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d3106-117">The app's description.</span></span>|
|<span data-ttu-id="d3106-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="d3106-118">publisherName</span></span>|<span data-ttu-id="d3106-119">String</span><span class="sxs-lookup"><span data-stu-id="d3106-119">String</span></span>|<span data-ttu-id="d3106-120">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="d3106-120">The publisher name</span></span>|
|<span data-ttu-id="d3106-121">productName</span><span class="sxs-lookup"><span data-stu-id="d3106-121">productName</span></span>|<span data-ttu-id="d3106-122">String</span><span class="sxs-lookup"><span data-stu-id="d3106-122">String</span></span>|<span data-ttu-id="d3106-123">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="d3106-123">The product name.</span></span>|
|<span data-ttu-id="d3106-124">denied</span><span class="sxs-lookup"><span data-stu-id="d3106-124">denied</span></span>|<span data-ttu-id="d3106-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3106-125">Boolean</span></span>|<span data-ttu-id="d3106-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="d3106-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3106-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d3106-127">Relationships</span></span>
<span data-ttu-id="d3106-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d3106-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3106-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3106-129">JSON Representation</span></span>
<span data-ttu-id="d3106-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3106-130">Here is a JSON representation of the resource.</span></span>
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




