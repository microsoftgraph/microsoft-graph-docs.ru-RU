---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97e1e866dc71b08064fe46878c25cb5b43c90177
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533331"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="55901-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="55901-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="55901-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55901-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55901-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55901-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55901-106">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="55901-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="55901-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="55901-107">Properties</span></span>
|<span data-ttu-id="55901-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="55901-108">Property</span></span>|<span data-ttu-id="55901-109">Тип</span><span class="sxs-lookup"><span data-stu-id="55901-109">Type</span></span>|<span data-ttu-id="55901-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55901-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55901-111">displayName</span><span class="sxs-lookup"><span data-stu-id="55901-111">displayName</span></span>|<span data-ttu-id="55901-112">Строка</span><span class="sxs-lookup"><span data-stu-id="55901-112">String</span></span>|<span data-ttu-id="55901-113">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="55901-113">App display name.</span></span>|
|<span data-ttu-id="55901-114">description</span><span class="sxs-lookup"><span data-stu-id="55901-114">description</span></span>|<span data-ttu-id="55901-115">Строка</span><span class="sxs-lookup"><span data-stu-id="55901-115">String</span></span>|<span data-ttu-id="55901-116">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="55901-116">The app's description.</span></span>|
|<span data-ttu-id="55901-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="55901-117">publisherName</span></span>|<span data-ttu-id="55901-118">String</span><span class="sxs-lookup"><span data-stu-id="55901-118">String</span></span>|<span data-ttu-id="55901-119">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="55901-119">The publisher name</span></span>|
|<span data-ttu-id="55901-120">productName</span><span class="sxs-lookup"><span data-stu-id="55901-120">productName</span></span>|<span data-ttu-id="55901-121">String</span><span class="sxs-lookup"><span data-stu-id="55901-121">String</span></span>|<span data-ttu-id="55901-122">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="55901-122">The product name.</span></span>|
|<span data-ttu-id="55901-123">denied</span><span class="sxs-lookup"><span data-stu-id="55901-123">denied</span></span>|<span data-ttu-id="55901-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="55901-124">Boolean</span></span>|<span data-ttu-id="55901-125">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="55901-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55901-126">Связи</span><span class="sxs-lookup"><span data-stu-id="55901-126">Relationships</span></span>
<span data-ttu-id="55901-127">Нет</span><span class="sxs-lookup"><span data-stu-id="55901-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55901-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55901-128">JSON Representation</span></span>
<span data-ttu-id="55901-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55901-129">Here is a JSON representation of the resource.</span></span>
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




