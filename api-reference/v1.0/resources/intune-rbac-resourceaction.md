---
title: Тип ресурса resourceAction
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 899075a8ac494daf345fa6f8d91e3cc38126ec53
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441625"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="ff54c-103">Тип ресурса resourceAction</span><span class="sxs-lookup"><span data-stu-id="ff54c-103">resourceAction resource type</span></span>

<span data-ttu-id="ff54c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff54c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff54c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff54c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff54c-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ff54c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ff54c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff54c-107">Properties</span></span>
|<span data-ttu-id="ff54c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff54c-108">Property</span></span>|<span data-ttu-id="ff54c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ff54c-109">Type</span></span>|<span data-ttu-id="ff54c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff54c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff54c-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="ff54c-111">allowedResourceActions</span></span>|<span data-ttu-id="ff54c-112">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="ff54c-112">String collection</span></span>|<span data-ttu-id="ff54c-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="ff54c-113">Allowed Actions</span></span>|
|<span data-ttu-id="ff54c-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="ff54c-114">notAllowedResourceActions</span></span>|<span data-ttu-id="ff54c-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ff54c-115">String collection</span></span>|<span data-ttu-id="ff54c-116">Запрещенные действия</span><span class="sxs-lookup"><span data-stu-id="ff54c-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff54c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="ff54c-117">Relationships</span></span>
<span data-ttu-id="ff54c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ff54c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff54c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff54c-119">JSON Representation</span></span>
<span data-ttu-id="ff54c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff54c-120">Here is a JSON representation of the resource.</span></span>
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







