---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba372cd3e8f67371adac9f92da92da4c7efe2a28
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525693"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="03029-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="03029-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="03029-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03029-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03029-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03029-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03029-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03029-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03029-107">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="03029-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="03029-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="03029-108">Properties</span></span>
|<span data-ttu-id="03029-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="03029-109">Property</span></span>|<span data-ttu-id="03029-110">Тип</span><span class="sxs-lookup"><span data-stu-id="03029-110">Type</span></span>|<span data-ttu-id="03029-111">Описание</span><span class="sxs-lookup"><span data-stu-id="03029-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03029-112">Тип</span><span class="sxs-lookup"><span data-stu-id="03029-112">appType</span></span>|[<span data-ttu-id="03029-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="03029-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="03029-114">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="03029-114">Application type.</span></span> <span data-ttu-id="03029-115">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="03029-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="03029-116">идентификатор</span><span class="sxs-lookup"><span data-stu-id="03029-116">identifier</span></span>|<span data-ttu-id="03029-117">String</span><span class="sxs-lookup"><span data-stu-id="03029-117">String</span></span>|<span data-ttu-id="03029-118">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="03029-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03029-119">Связи</span><span class="sxs-lookup"><span data-stu-id="03029-119">Relationships</span></span>
<span data-ttu-id="03029-120">Нет</span><span class="sxs-lookup"><span data-stu-id="03029-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03029-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03029-121">JSON Representation</span></span>
<span data-ttu-id="03029-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03029-122">Here is a JSON representation of the resource.</span></span>
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



