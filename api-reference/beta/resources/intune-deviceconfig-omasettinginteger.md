---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1b0dc774d5ab95733337719014f9db93bc393d71
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462990"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="8474b-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="8474b-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="8474b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8474b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8474b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8474b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8474b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8474b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8474b-107">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="8474b-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="8474b-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8474b-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8474b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8474b-109">Properties</span></span>
|<span data-ttu-id="8474b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8474b-110">Property</span></span>|<span data-ttu-id="8474b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8474b-111">Type</span></span>|<span data-ttu-id="8474b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8474b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8474b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="8474b-113">displayName</span></span>|<span data-ttu-id="8474b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="8474b-114">String</span></span>|<span data-ttu-id="8474b-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="8474b-115">Display Name.</span></span> <span data-ttu-id="8474b-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8474b-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8474b-117">description</span><span class="sxs-lookup"><span data-stu-id="8474b-117">description</span></span>|<span data-ttu-id="8474b-118">String</span><span class="sxs-lookup"><span data-stu-id="8474b-118">String</span></span>|<span data-ttu-id="8474b-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="8474b-119">Description.</span></span> <span data-ttu-id="8474b-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8474b-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8474b-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="8474b-121">omaUri</span></span>|<span data-ttu-id="8474b-122">String</span><span class="sxs-lookup"><span data-stu-id="8474b-122">String</span></span>|<span data-ttu-id="8474b-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="8474b-123">OMA.</span></span> <span data-ttu-id="8474b-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8474b-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8474b-125">value</span><span class="sxs-lookup"><span data-stu-id="8474b-125">value</span></span>|<span data-ttu-id="8474b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="8474b-126">Int32</span></span>|<span data-ttu-id="8474b-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="8474b-127">Value.</span></span>|
|<span data-ttu-id="8474b-128">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="8474b-128">isReadOnly</span></span>|<span data-ttu-id="8474b-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="8474b-129">Boolean</span></span>|<span data-ttu-id="8474b-130">Если задано значение true, CSP (поставщик услуг по настройке), указанный в OMA-URI, будет выполнять Get, а не Set</span><span class="sxs-lookup"><span data-stu-id="8474b-130">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="8474b-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="8474b-131">Relationships</span></span>
<span data-ttu-id="8474b-132">Нет</span><span class="sxs-lookup"><span data-stu-id="8474b-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8474b-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8474b-133">JSON Representation</span></span>
<span data-ttu-id="8474b-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8474b-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024,
  "isReadOnly": true
}
```



