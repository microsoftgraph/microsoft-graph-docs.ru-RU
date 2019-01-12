---
title: Тип ресурса windowsInformationProtectionApp
description: Защита данных приложений для Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 270dd0b6328cd8290e656e46a0ff40551d2a5cbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917799"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="23aa1-103">Тип ресурса windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="23aa1-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="23aa1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23aa1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23aa1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23aa1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23aa1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23aa1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23aa1-107">Защита данных приложений для Windows</span><span class="sxs-lookup"><span data-stu-id="23aa1-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="23aa1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="23aa1-108">Properties</span></span>
|<span data-ttu-id="23aa1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="23aa1-109">Property</span></span>|<span data-ttu-id="23aa1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="23aa1-110">Type</span></span>|<span data-ttu-id="23aa1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23aa1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23aa1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="23aa1-112">displayName</span></span>|<span data-ttu-id="23aa1-113">String</span><span class="sxs-lookup"><span data-stu-id="23aa1-113">String</span></span>|<span data-ttu-id="23aa1-114">Отображаемое имя приложения.</span><span class="sxs-lookup"><span data-stu-id="23aa1-114">App display name.</span></span>|
|<span data-ttu-id="23aa1-115">описание</span><span class="sxs-lookup"><span data-stu-id="23aa1-115">description</span></span>|<span data-ttu-id="23aa1-116">String</span><span class="sxs-lookup"><span data-stu-id="23aa1-116">String</span></span>|<span data-ttu-id="23aa1-117">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="23aa1-117">The app's description.</span></span>|
|<span data-ttu-id="23aa1-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="23aa1-118">publisherName</span></span>|<span data-ttu-id="23aa1-119">String</span><span class="sxs-lookup"><span data-stu-id="23aa1-119">String</span></span>|<span data-ttu-id="23aa1-120">Имя издателя</span><span class="sxs-lookup"><span data-stu-id="23aa1-120">The publisher name</span></span>|
|<span data-ttu-id="23aa1-121">productName</span><span class="sxs-lookup"><span data-stu-id="23aa1-121">productName</span></span>|<span data-ttu-id="23aa1-122">String</span><span class="sxs-lookup"><span data-stu-id="23aa1-122">String</span></span>|<span data-ttu-id="23aa1-123">Название продукта.</span><span class="sxs-lookup"><span data-stu-id="23aa1-123">The product name.</span></span>|
|<span data-ttu-id="23aa1-124">denied</span><span class="sxs-lookup"><span data-stu-id="23aa1-124">denied</span></span>|<span data-ttu-id="23aa1-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="23aa1-125">Boolean</span></span>|<span data-ttu-id="23aa1-126">Если задано значение true, то приложению отказано в защите или исключении.</span><span class="sxs-lookup"><span data-stu-id="23aa1-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23aa1-127">Связи</span><span class="sxs-lookup"><span data-stu-id="23aa1-127">Relationships</span></span>
<span data-ttu-id="23aa1-128">Нет</span><span class="sxs-lookup"><span data-stu-id="23aa1-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23aa1-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23aa1-129">JSON Representation</span></span>
<span data-ttu-id="23aa1-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23aa1-130">Here is a JSON representation of the resource.</span></span>
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





