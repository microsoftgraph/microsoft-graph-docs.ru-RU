---
title: Тип ресурса Девицехеалсскриптпараметер
description: Базовые свойства параметра скрипта.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad82da1915702448a62c0c99f6933ddf1a51c5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060302"
---
# <a name="devicehealthscriptparameter-resource-type"></a><span data-ttu-id="29ddb-103">Тип ресурса Девицехеалсскриптпараметер</span><span class="sxs-lookup"><span data-stu-id="29ddb-103">deviceHealthScriptParameter resource type</span></span>

<span data-ttu-id="29ddb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29ddb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29ddb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ddb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29ddb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="29ddb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29ddb-107">Базовые свойства параметра скрипта.</span><span class="sxs-lookup"><span data-stu-id="29ddb-107">Base properties of the script parameter.</span></span>

## <a name="properties"></a><span data-ttu-id="29ddb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="29ddb-108">Properties</span></span>
|<span data-ttu-id="29ddb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="29ddb-109">Property</span></span>|<span data-ttu-id="29ddb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="29ddb-110">Type</span></span>|<span data-ttu-id="29ddb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="29ddb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29ddb-112">name</span><span class="sxs-lookup"><span data-stu-id="29ddb-112">name</span></span>|<span data-ttu-id="29ddb-113">String</span><span class="sxs-lookup"><span data-stu-id="29ddb-113">String</span></span>|<span data-ttu-id="29ddb-114">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="29ddb-114">The name of the param</span></span>|
|<span data-ttu-id="29ddb-115">description</span><span class="sxs-lookup"><span data-stu-id="29ddb-115">description</span></span>|<span data-ttu-id="29ddb-116">String</span><span class="sxs-lookup"><span data-stu-id="29ddb-116">String</span></span>|<span data-ttu-id="29ddb-117">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="29ddb-117">The description of the param</span></span>|
|<span data-ttu-id="29ddb-118">isRequired</span><span class="sxs-lookup"><span data-stu-id="29ddb-118">isRequired</span></span>|<span data-ttu-id="29ddb-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="29ddb-119">Boolean</span></span>|<span data-ttu-id="29ddb-120">Является ли параметр обязательным</span><span class="sxs-lookup"><span data-stu-id="29ddb-120">Whether the param is required</span></span>|
|<span data-ttu-id="29ddb-121">апплидефаултвалуевхеннотассигнед</span><span class="sxs-lookup"><span data-stu-id="29ddb-121">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="29ddb-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="29ddb-122">Boolean</span></span>|<span data-ttu-id="29ddb-123">Применяется ли значение DefaultValue при отсутствии назначения</span><span class="sxs-lookup"><span data-stu-id="29ddb-123">Whether Apply DefaultValue When Not Assigned</span></span>|

## <a name="relationships"></a><span data-ttu-id="29ddb-124">Связи</span><span class="sxs-lookup"><span data-stu-id="29ddb-124">Relationships</span></span>
<span data-ttu-id="29ddb-125">Нет</span><span class="sxs-lookup"><span data-stu-id="29ddb-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29ddb-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29ddb-126">JSON Representation</span></span>
<span data-ttu-id="29ddb-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29ddb-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true
}
```






