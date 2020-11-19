---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67ab2980b8fb228803eee955302f9db69065dd15
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273090"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="38dda-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="38dda-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="38dda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38dda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38dda-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38dda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38dda-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38dda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38dda-107">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="38dda-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="38dda-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38dda-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38dda-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="38dda-109">Properties</span></span>
|<span data-ttu-id="38dda-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="38dda-110">Property</span></span>|<span data-ttu-id="38dda-111">Тип</span><span class="sxs-lookup"><span data-stu-id="38dda-111">Type</span></span>|<span data-ttu-id="38dda-112">Описание</span><span class="sxs-lookup"><span data-stu-id="38dda-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38dda-113">displayName</span><span class="sxs-lookup"><span data-stu-id="38dda-113">displayName</span></span>|<span data-ttu-id="38dda-114">String</span><span class="sxs-lookup"><span data-stu-id="38dda-114">String</span></span>|<span data-ttu-id="38dda-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="38dda-115">Display Name.</span></span> <span data-ttu-id="38dda-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38dda-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38dda-117">description</span><span class="sxs-lookup"><span data-stu-id="38dda-117">description</span></span>|<span data-ttu-id="38dda-118">String</span><span class="sxs-lookup"><span data-stu-id="38dda-118">String</span></span>|<span data-ttu-id="38dda-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="38dda-119">Description.</span></span> <span data-ttu-id="38dda-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38dda-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38dda-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="38dda-121">omaUri</span></span>|<span data-ttu-id="38dda-122">String</span><span class="sxs-lookup"><span data-stu-id="38dda-122">String</span></span>|<span data-ttu-id="38dda-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="38dda-123">OMA.</span></span> <span data-ttu-id="38dda-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38dda-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38dda-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="38dda-125">isEncrypted</span></span>|<span data-ttu-id="38dda-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="38dda-126">Boolean</span></span>|<span data-ttu-id="38dda-127">Указывает, зашифровано ли поле "значение".</span><span class="sxs-lookup"><span data-stu-id="38dda-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="38dda-128">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38dda-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="38dda-129">value</span><span class="sxs-lookup"><span data-stu-id="38dda-129">value</span></span>|<span data-ttu-id="38dda-130">Int32</span><span class="sxs-lookup"><span data-stu-id="38dda-130">Int32</span></span>|<span data-ttu-id="38dda-131">Значение.</span><span class="sxs-lookup"><span data-stu-id="38dda-131">Value.</span></span>|
|<span data-ttu-id="38dda-132">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="38dda-132">isReadOnly</span></span>|<span data-ttu-id="38dda-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="38dda-133">Boolean</span></span>|<span data-ttu-id="38dda-134">Если задано значение true, CSP (поставщик услуг по настройке), указанный в OMA-URI, будет выполнять Get, а не Set</span><span class="sxs-lookup"><span data-stu-id="38dda-134">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="38dda-135">Связи</span><span class="sxs-lookup"><span data-stu-id="38dda-135">Relationships</span></span>
<span data-ttu-id="38dda-136">Нет</span><span class="sxs-lookup"><span data-stu-id="38dda-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38dda-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38dda-137">JSON Representation</span></span>
<span data-ttu-id="38dda-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38dda-138">Here is a JSON representation of the resource.</span></span>
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
  "isEncrypted": true,
  "value": 1024,
  "isReadOnly": true
}
```




