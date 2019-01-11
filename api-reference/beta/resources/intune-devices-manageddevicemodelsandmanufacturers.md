---
title: Тип ресурса managedDeviceModelsAndManufacturers
description: Модели и производители meatadata для управляемых устройств в учетной записи
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86d9f9dd0642abab73f6b750b997c75851f6be02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875623"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="4a9e2-103">Тип ресурса managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="4a9e2-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="4a9e2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4a9e2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a9e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a9e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a9e2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4a9e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a9e2-107">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="4a9e2-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="4a9e2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a9e2-108">Properties</span></span>
|<span data-ttu-id="4a9e2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a9e2-109">Property</span></span>|<span data-ttu-id="4a9e2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4a9e2-110">Type</span></span>|<span data-ttu-id="4a9e2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a9e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a9e2-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="4a9e2-112">deviceModels</span></span>|<span data-ttu-id="4a9e2-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a9e2-113">String collection</span></span>|<span data-ttu-id="4a9e2-114">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="4a9e2-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="4a9e2-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="4a9e2-115">deviceManufacturers</span></span>|<span data-ttu-id="4a9e2-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a9e2-116">String collection</span></span>|<span data-ttu-id="4a9e2-117">Список производители управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="4a9e2-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a9e2-118">Связи</span><span class="sxs-lookup"><span data-stu-id="4a9e2-118">Relationships</span></span>
<span data-ttu-id="4a9e2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="4a9e2-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a9e2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a9e2-120">JSON Representation</span></span>
<span data-ttu-id="4a9e2-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a9e2-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```





