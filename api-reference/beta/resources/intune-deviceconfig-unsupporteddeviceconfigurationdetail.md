---
title: Тип ресурса unsupportedDeviceConfigurationDetail
description: Описание причины сущности не поддерживается.
author: tfitzmac
ms.openlocfilehash: 4cccf49366a803e5f964605a4dc4ba7f56707823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344053"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="3565d-103">Тип ресурса unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="3565d-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="3565d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3565d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3565d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3565d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3565d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3565d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3565d-107">Описание причины сущности не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3565d-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="3565d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3565d-108">Properties</span></span>
|<span data-ttu-id="3565d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3565d-109">Property</span></span>|<span data-ttu-id="3565d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3565d-110">Type</span></span>|<span data-ttu-id="3565d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3565d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3565d-112">message</span><span class="sxs-lookup"><span data-stu-id="3565d-112">message</span></span>|<span data-ttu-id="3565d-113">String</span><span class="sxs-lookup"><span data-stu-id="3565d-113">String</span></span>|<span data-ttu-id="3565d-114">Сообщение о том, почему сущности не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3565d-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="3565d-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="3565d-115">propertyName</span></span>|<span data-ttu-id="3565d-116">String.</span><span class="sxs-lookup"><span data-stu-id="3565d-116">String</span></span>|<span data-ttu-id="3565d-117">Если сообщение относится к определенное свойство в исходной сущности, а затем имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="3565d-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3565d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3565d-118">Relationships</span></span>
<span data-ttu-id="3565d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3565d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3565d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3565d-120">JSON Representation</span></span>
<span data-ttu-id="3565d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3565d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```





