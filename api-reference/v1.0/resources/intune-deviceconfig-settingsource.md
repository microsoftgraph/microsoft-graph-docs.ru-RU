---
title: Тип ресурса settingSource
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2cfe802c344550fa15c84614911db55493e93125
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759975"
---
# <a name="settingsource-resource-type"></a><span data-ttu-id="54dde-103">Тип ресурса settingSource</span><span class="sxs-lookup"><span data-stu-id="54dde-103">settingSource resource type</span></span>

<span data-ttu-id="54dde-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54dde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54dde-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54dde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54dde-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="54dde-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="54dde-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54dde-107">Properties</span></span>
|<span data-ttu-id="54dde-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54dde-108">Property</span></span>|<span data-ttu-id="54dde-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54dde-109">Type</span></span>|<span data-ttu-id="54dde-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54dde-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54dde-111">id</span><span class="sxs-lookup"><span data-stu-id="54dde-111">id</span></span>|<span data-ttu-id="54dde-112">String</span><span class="sxs-lookup"><span data-stu-id="54dde-112">String</span></span>|<span data-ttu-id="54dde-113">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="54dde-113">Not yet documented</span></span>|
|<span data-ttu-id="54dde-114">displayName</span><span class="sxs-lookup"><span data-stu-id="54dde-114">displayName</span></span>|<span data-ttu-id="54dde-115">String</span><span class="sxs-lookup"><span data-stu-id="54dde-115">String</span></span>|<span data-ttu-id="54dde-116">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="54dde-116">Not yet documented</span></span>|
|<span data-ttu-id="54dde-117">sourceType</span><span class="sxs-lookup"><span data-stu-id="54dde-117">sourceType</span></span>|[<span data-ttu-id="54dde-118">settingSourceType</span><span class="sxs-lookup"><span data-stu-id="54dde-118">settingSourceType</span></span>](../resources/intune-deviceconfig-settingsourcetype.md)|<span data-ttu-id="54dde-119">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="54dde-119">Not yet documented.</span></span> <span data-ttu-id="54dde-120">Возможные значения: `deviceConfiguration`, `deviceIntent`.</span><span class="sxs-lookup"><span data-stu-id="54dde-120">Possible values are: `deviceConfiguration`, `deviceIntent`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54dde-121">Связи</span><span class="sxs-lookup"><span data-stu-id="54dde-121">Relationships</span></span>
<span data-ttu-id="54dde-122">Нет</span><span class="sxs-lookup"><span data-stu-id="54dde-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54dde-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54dde-123">JSON Representation</span></span>
<span data-ttu-id="54dde-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54dde-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.settingSource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingSource",
  "id": "String (identifier)",
  "displayName": "String",
  "sourceType": "String"
}
```




