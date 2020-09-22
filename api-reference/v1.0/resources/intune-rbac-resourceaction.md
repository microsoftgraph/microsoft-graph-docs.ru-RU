---
title: Тип ресурса resourceAction
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 941ebf1c7a56e04acaa118bf0d0ed8594172c726
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037810"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="09b00-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="09b00-103">resourceAction resource type</span></span>

<span data-ttu-id="09b00-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09b00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09b00-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09b00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09b00-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="09b00-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="09b00-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="09b00-107">Properties</span></span>
|<span data-ttu-id="09b00-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="09b00-108">Property</span></span>|<span data-ttu-id="09b00-109">Тип</span><span class="sxs-lookup"><span data-stu-id="09b00-109">Type</span></span>|<span data-ttu-id="09b00-110">Описание</span><span class="sxs-lookup"><span data-stu-id="09b00-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09b00-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="09b00-111">allowedResourceActions</span></span>|<span data-ttu-id="09b00-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="09b00-112">String collection</span></span>|<span data-ttu-id="09b00-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="09b00-113">Allowed Actions</span></span>|
|<span data-ttu-id="09b00-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="09b00-114">notAllowedResourceActions</span></span>|<span data-ttu-id="09b00-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="09b00-115">String collection</span></span>|<span data-ttu-id="09b00-116">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="09b00-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="09b00-117">Связи</span><span class="sxs-lookup"><span data-stu-id="09b00-117">Relationships</span></span>
<span data-ttu-id="09b00-118">Нет</span><span class="sxs-lookup"><span data-stu-id="09b00-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09b00-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09b00-119">JSON Representation</span></span>
<span data-ttu-id="09b00-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09b00-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```









