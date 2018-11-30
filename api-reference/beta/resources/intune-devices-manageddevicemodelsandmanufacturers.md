---
title: Тип ресурса managedDeviceModelsAndManufacturers
description: Модели и производители meatadata для управляемых устройств в учетной записи
ms.openlocfilehash: c61026a6caa097e01e09a4343dd54f769c743460
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082611"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="6397a-103">Тип ресурса managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="6397a-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="6397a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6397a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6397a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6397a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6397a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6397a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6397a-107">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="6397a-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="6397a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6397a-108">Properties</span></span>
|<span data-ttu-id="6397a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6397a-109">Property</span></span>|<span data-ttu-id="6397a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6397a-110">Type</span></span>|<span data-ttu-id="6397a-111">Description</span><span class="sxs-lookup"><span data-stu-id="6397a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6397a-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="6397a-112">deviceModels</span></span>|<span data-ttu-id="6397a-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6397a-113">String collection</span></span>|<span data-ttu-id="6397a-114">Список моделей для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="6397a-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="6397a-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="6397a-115">deviceManufacturers</span></span>|<span data-ttu-id="6397a-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6397a-116">String collection</span></span>|<span data-ttu-id="6397a-117">Список производители управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="6397a-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="6397a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="6397a-118">Relationships</span></span>
<span data-ttu-id="6397a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6397a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6397a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6397a-120">JSON Representation</span></span>
<span data-ttu-id="6397a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6397a-121">Here is a JSON representation of the resource.</span></span>
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





