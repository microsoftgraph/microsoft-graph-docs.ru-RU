---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2487abe38ca73c82994e9341ed21dce2e0941a5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732504"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="8bc93-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="8bc93-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="8bc93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bc93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bc93-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bc93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bc93-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bc93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc93-107">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="8bc93-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8bc93-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bc93-108">Properties</span></span>
|<span data-ttu-id="8bc93-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bc93-109">Property</span></span>|<span data-ttu-id="8bc93-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8bc93-110">Type</span></span>|<span data-ttu-id="8bc93-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8bc93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc93-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8bc93-112">appType</span></span>|[<span data-ttu-id="8bc93-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="8bc93-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="8bc93-114">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="8bc93-114">Application type.</span></span> <span data-ttu-id="8bc93-115">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="8bc93-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="8bc93-116">идентификатор</span><span class="sxs-lookup"><span data-stu-id="8bc93-116">identifier</span></span>|<span data-ttu-id="8bc93-117">Строка</span><span class="sxs-lookup"><span data-stu-id="8bc93-117">String</span></span>|<span data-ttu-id="8bc93-118">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="8bc93-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bc93-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8bc93-119">Relationships</span></span>
<span data-ttu-id="8bc93-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8bc93-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bc93-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bc93-121">JSON Representation</span></span>
<span data-ttu-id="8bc93-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bc93-122">Here is a JSON representation of the resource.</span></span>
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





