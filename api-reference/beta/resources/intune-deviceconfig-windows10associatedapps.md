---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ecdea1d1493388c1fab3037d49b41f5f3388e3c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985918"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="d93b5-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="d93b5-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="d93b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d93b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d93b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d93b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d93b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d93b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d93b5-107">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d93b5-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d93b5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d93b5-108">Properties</span></span>
|<span data-ttu-id="d93b5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d93b5-109">Property</span></span>|<span data-ttu-id="d93b5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d93b5-110">Type</span></span>|<span data-ttu-id="d93b5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d93b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d93b5-112">Тип</span><span class="sxs-lookup"><span data-stu-id="d93b5-112">appType</span></span>|[<span data-ttu-id="d93b5-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="d93b5-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="d93b5-114">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="d93b5-114">Application type.</span></span> <span data-ttu-id="d93b5-115">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="d93b5-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="d93b5-116">идентификатор</span><span class="sxs-lookup"><span data-stu-id="d93b5-116">identifier</span></span>|<span data-ttu-id="d93b5-117">String</span><span class="sxs-lookup"><span data-stu-id="d93b5-117">String</span></span>|<span data-ttu-id="d93b5-118">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="d93b5-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d93b5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="d93b5-119">Relationships</span></span>
<span data-ttu-id="d93b5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d93b5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d93b5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d93b5-121">JSON Representation</span></span>
<span data-ttu-id="d93b5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d93b5-122">Here is a JSON representation of the resource.</span></span>
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






