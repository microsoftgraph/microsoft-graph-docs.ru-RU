---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: tfitzmac
ms.openlocfilehash: 6ad47301dc7ec9650026021a2131d34b4d704e70
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334386"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="ed3f0-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="ed3f0-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="ed3f0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed3f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed3f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed3f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed3f0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed3f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed3f0-107">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="ed3f0-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="ed3f0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed3f0-108">Properties</span></span>
|<span data-ttu-id="ed3f0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed3f0-109">Property</span></span>|<span data-ttu-id="ed3f0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ed3f0-110">Type</span></span>|<span data-ttu-id="ed3f0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed3f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed3f0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ed3f0-112">displayName</span></span>|<span data-ttu-id="ed3f0-113">String</span><span class="sxs-lookup"><span data-stu-id="ed3f0-113">String</span></span>|<span data-ttu-id="ed3f0-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="ed3f0-114">App display name.</span></span>|
|<span data-ttu-id="ed3f0-115">описание</span><span class="sxs-lookup"><span data-stu-id="ed3f0-115">description</span></span>|<span data-ttu-id="ed3f0-116">String</span><span class="sxs-lookup"><span data-stu-id="ed3f0-116">String</span></span>|<span data-ttu-id="ed3f0-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ed3f0-117">The app's description.</span></span>|
|<span data-ttu-id="ed3f0-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="ed3f0-118">publisherName</span></span>|<span data-ttu-id="ed3f0-119">String</span><span class="sxs-lookup"><span data-stu-id="ed3f0-119">String</span></span>|<span data-ttu-id="ed3f0-120">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="ed3f0-120">The publisher name</span></span>|
|<span data-ttu-id="ed3f0-121">productName</span><span class="sxs-lookup"><span data-stu-id="ed3f0-121">productName</span></span>|<span data-ttu-id="ed3f0-122">String</span><span class="sxs-lookup"><span data-stu-id="ed3f0-122">String</span></span>|<span data-ttu-id="ed3f0-123">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="ed3f0-123">The product name.</span></span>|
|<span data-ttu-id="ed3f0-124">denied</span><span class="sxs-lookup"><span data-stu-id="ed3f0-124">denied</span></span>|<span data-ttu-id="ed3f0-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed3f0-125">Boolean</span></span>|<span data-ttu-id="ed3f0-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="ed3f0-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed3f0-127">Связи</span><span class="sxs-lookup"><span data-stu-id="ed3f0-127">Relationships</span></span>
<span data-ttu-id="ed3f0-128">Нет</span><span class="sxs-lookup"><span data-stu-id="ed3f0-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed3f0-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed3f0-129">JSON Representation</span></span>
<span data-ttu-id="ed3f0-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed3f0-130">Here is a JSON representation of the resource.</span></span>
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





