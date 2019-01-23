---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения связанного 10 Windows.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5dd5b664bde2970caa4b09c027592684b9ecd5e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425920"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="d024d-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="d024d-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="d024d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d024d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d024d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d024d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d024d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d024d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d024d-107">Определение приложения связанного 10 Windows.</span><span class="sxs-lookup"><span data-stu-id="d024d-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d024d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d024d-108">Properties</span></span>
|<span data-ttu-id="d024d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d024d-109">Property</span></span>|<span data-ttu-id="d024d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d024d-110">Type</span></span>|<span data-ttu-id="d024d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d024d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d024d-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d024d-112">appType</span></span>|[<span data-ttu-id="d024d-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="d024d-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="d024d-114">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="d024d-114">Application type.</span></span> <span data-ttu-id="d024d-115">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="d024d-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="d024d-116">идентификатор</span><span class="sxs-lookup"><span data-stu-id="d024d-116">identifier</span></span>|<span data-ttu-id="d024d-117">String</span><span class="sxs-lookup"><span data-stu-id="d024d-117">String</span></span>|<span data-ttu-id="d024d-118">Идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d024d-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d024d-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="d024d-119">Relationships</span></span>
<span data-ttu-id="d024d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d024d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d024d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d024d-121">JSON Representation</span></span>
<span data-ttu-id="d024d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d024d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```




