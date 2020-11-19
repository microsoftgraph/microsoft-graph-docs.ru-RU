---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1f17f03a553b5040eab7ac482ad4b13d54bbf69
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279670"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="bd405-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="bd405-103">omaSettingString resource type</span></span>

<span data-ttu-id="bd405-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd405-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd405-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd405-107">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="bd405-107">OMA Settings String definition.</span></span>


<span data-ttu-id="bd405-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd405-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd405-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd405-109">Properties</span></span>
|<span data-ttu-id="bd405-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd405-110">Property</span></span>|<span data-ttu-id="bd405-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bd405-111">Type</span></span>|<span data-ttu-id="bd405-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bd405-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd405-113">displayName</span><span class="sxs-lookup"><span data-stu-id="bd405-113">displayName</span></span>|<span data-ttu-id="bd405-114">String</span><span class="sxs-lookup"><span data-stu-id="bd405-114">String</span></span>|<span data-ttu-id="bd405-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="bd405-115">Display Name.</span></span> <span data-ttu-id="bd405-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd405-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bd405-117">description</span><span class="sxs-lookup"><span data-stu-id="bd405-117">description</span></span>|<span data-ttu-id="bd405-118">String</span><span class="sxs-lookup"><span data-stu-id="bd405-118">String</span></span>|<span data-ttu-id="bd405-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="bd405-119">Description.</span></span> <span data-ttu-id="bd405-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd405-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bd405-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="bd405-121">omaUri</span></span>|<span data-ttu-id="bd405-122">String</span><span class="sxs-lookup"><span data-stu-id="bd405-122">String</span></span>|<span data-ttu-id="bd405-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="bd405-123">OMA.</span></span> <span data-ttu-id="bd405-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd405-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bd405-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="bd405-125">isEncrypted</span></span>|<span data-ttu-id="bd405-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd405-126">Boolean</span></span>|<span data-ttu-id="bd405-127">Указывает, зашифровано ли поле "значение".</span><span class="sxs-lookup"><span data-stu-id="bd405-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="bd405-128">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bd405-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bd405-129">value</span><span class="sxs-lookup"><span data-stu-id="bd405-129">value</span></span>|<span data-ttu-id="bd405-130">String</span><span class="sxs-lookup"><span data-stu-id="bd405-130">String</span></span>|<span data-ttu-id="bd405-131">Значение</span><span class="sxs-lookup"><span data-stu-id="bd405-131">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd405-132">Связи</span><span class="sxs-lookup"><span data-stu-id="bd405-132">Relationships</span></span>
<span data-ttu-id="bd405-133">Нет</span><span class="sxs-lookup"><span data-stu-id="bd405-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd405-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd405-134">JSON Representation</span></span>
<span data-ttu-id="bd405-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd405-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "isEncrypted": true,
  "value": "String"
}
```




