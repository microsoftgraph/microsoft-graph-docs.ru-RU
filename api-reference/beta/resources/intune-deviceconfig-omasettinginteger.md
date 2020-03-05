---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5c6f4c79092b04e749a4625cfa590578058a2ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529554"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="97b47-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="97b47-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="97b47-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="97b47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97b47-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97b47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97b47-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97b47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97b47-107">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="97b47-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="97b47-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="97b47-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97b47-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="97b47-109">Properties</span></span>
|<span data-ttu-id="97b47-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="97b47-110">Property</span></span>|<span data-ttu-id="97b47-111">Тип</span><span class="sxs-lookup"><span data-stu-id="97b47-111">Type</span></span>|<span data-ttu-id="97b47-112">Описание</span><span class="sxs-lookup"><span data-stu-id="97b47-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97b47-113">displayName</span><span class="sxs-lookup"><span data-stu-id="97b47-113">displayName</span></span>|<span data-ttu-id="97b47-114">Строка</span><span class="sxs-lookup"><span data-stu-id="97b47-114">String</span></span>|<span data-ttu-id="97b47-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="97b47-115">Display Name.</span></span> <span data-ttu-id="97b47-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="97b47-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="97b47-117">description</span><span class="sxs-lookup"><span data-stu-id="97b47-117">description</span></span>|<span data-ttu-id="97b47-118">String</span><span class="sxs-lookup"><span data-stu-id="97b47-118">String</span></span>|<span data-ttu-id="97b47-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="97b47-119">Description.</span></span> <span data-ttu-id="97b47-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="97b47-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="97b47-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="97b47-121">omaUri</span></span>|<span data-ttu-id="97b47-122">String</span><span class="sxs-lookup"><span data-stu-id="97b47-122">String</span></span>|<span data-ttu-id="97b47-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="97b47-123">OMA.</span></span> <span data-ttu-id="97b47-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="97b47-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="97b47-125">value</span><span class="sxs-lookup"><span data-stu-id="97b47-125">value</span></span>|<span data-ttu-id="97b47-126">Int32</span><span class="sxs-lookup"><span data-stu-id="97b47-126">Int32</span></span>|<span data-ttu-id="97b47-127">Значение.</span><span class="sxs-lookup"><span data-stu-id="97b47-127">Value.</span></span>|
|<span data-ttu-id="97b47-128">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="97b47-128">isReadOnly</span></span>|<span data-ttu-id="97b47-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="97b47-129">Boolean</span></span>|<span data-ttu-id="97b47-130">Если задано значение true, CSP (поставщик услуг по настройке), указанный в OMA-URI, будет выполнять Get, а не Set</span><span class="sxs-lookup"><span data-stu-id="97b47-130">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="97b47-131">Связи</span><span class="sxs-lookup"><span data-stu-id="97b47-131">Relationships</span></span>
<span data-ttu-id="97b47-132">Нет</span><span class="sxs-lookup"><span data-stu-id="97b47-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97b47-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97b47-133">JSON Representation</span></span>
<span data-ttu-id="97b47-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97b47-134">Here is a JSON representation of the resource.</span></span>
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



