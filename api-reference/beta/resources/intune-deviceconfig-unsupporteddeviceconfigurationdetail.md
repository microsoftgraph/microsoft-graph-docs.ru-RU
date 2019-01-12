---
title: Тип ресурса unsupportedDeviceConfigurationDetail
description: Описание причины сущности не поддерживается.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6b82dcf28652cbe54a4932a641579101cb392639
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949775"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="a5d92-103">Тип ресурса unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="a5d92-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="a5d92-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5d92-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5d92-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5d92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5d92-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a5d92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5d92-107">Описание причины сущности не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5d92-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="a5d92-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5d92-108">Properties</span></span>
|<span data-ttu-id="a5d92-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5d92-109">Property</span></span>|<span data-ttu-id="a5d92-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a5d92-110">Type</span></span>|<span data-ttu-id="a5d92-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5d92-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5d92-112">message</span><span class="sxs-lookup"><span data-stu-id="a5d92-112">message</span></span>|<span data-ttu-id="a5d92-113">String</span><span class="sxs-lookup"><span data-stu-id="a5d92-113">String</span></span>|<span data-ttu-id="a5d92-114">Сообщение о том, почему сущности не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5d92-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="a5d92-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="a5d92-115">propertyName</span></span>|<span data-ttu-id="a5d92-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a5d92-116">String</span></span>|<span data-ttu-id="a5d92-117">Если сообщение относится к определенное свойство в исходной сущности, а затем имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="a5d92-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5d92-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a5d92-118">Relationships</span></span>
<span data-ttu-id="a5d92-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a5d92-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a5d92-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5d92-120">JSON Representation</span></span>
<span data-ttu-id="a5d92-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5d92-121">Here is a JSON representation of the resource.</span></span>
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





