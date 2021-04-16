---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e335f0e99b342df6c596900aab8f1a1933703b9f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867422"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="0cf68-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="0cf68-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="0cf68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cf68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cf68-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cf68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cf68-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cf68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cf68-107">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="0cf68-107">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="0cf68-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0cf68-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0cf68-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cf68-109">Properties</span></span>
|<span data-ttu-id="0cf68-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cf68-110">Property</span></span>|<span data-ttu-id="0cf68-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0cf68-111">Type</span></span>|<span data-ttu-id="0cf68-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0cf68-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cf68-113">displayName</span><span class="sxs-lookup"><span data-stu-id="0cf68-113">displayName</span></span>|<span data-ttu-id="0cf68-114">String</span><span class="sxs-lookup"><span data-stu-id="0cf68-114">String</span></span>|<span data-ttu-id="0cf68-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0cf68-115">Display Name.</span></span> <span data-ttu-id="0cf68-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0cf68-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0cf68-117">description</span><span class="sxs-lookup"><span data-stu-id="0cf68-117">description</span></span>|<span data-ttu-id="0cf68-118">String</span><span class="sxs-lookup"><span data-stu-id="0cf68-118">String</span></span>|<span data-ttu-id="0cf68-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="0cf68-119">Description.</span></span> <span data-ttu-id="0cf68-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0cf68-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0cf68-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="0cf68-121">omaUri</span></span>|<span data-ttu-id="0cf68-122">String</span><span class="sxs-lookup"><span data-stu-id="0cf68-122">String</span></span>|<span data-ttu-id="0cf68-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="0cf68-123">OMA.</span></span> <span data-ttu-id="0cf68-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0cf68-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0cf68-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="0cf68-125">secretReferenceValueId</span></span>|<span data-ttu-id="0cf68-126">String</span><span class="sxs-lookup"><span data-stu-id="0cf68-126">String</span></span>|<span data-ttu-id="0cf68-127">ReferenceId для поисков секрета для расшифровки.</span><span class="sxs-lookup"><span data-stu-id="0cf68-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="0cf68-128">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0cf68-128">This property is read-only.</span></span> <span data-ttu-id="0cf68-129">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0cf68-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0cf68-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="0cf68-130">isEncrypted</span></span>|<span data-ttu-id="0cf68-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cf68-131">Boolean</span></span>|<span data-ttu-id="0cf68-132">Указывает, зашифровано ли поле значений.</span><span class="sxs-lookup"><span data-stu-id="0cf68-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="0cf68-133">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0cf68-133">This property is read-only.</span></span> <span data-ttu-id="0cf68-134">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0cf68-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0cf68-135">value</span><span class="sxs-lookup"><span data-stu-id="0cf68-135">value</span></span>|<span data-ttu-id="0cf68-136">Single</span><span class="sxs-lookup"><span data-stu-id="0cf68-136">Single</span></span>|<span data-ttu-id="0cf68-137">Значение.</span><span class="sxs-lookup"><span data-stu-id="0cf68-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cf68-138">Связи</span><span class="sxs-lookup"><span data-stu-id="0cf68-138">Relationships</span></span>
<span data-ttu-id="0cf68-139">Нет</span><span class="sxs-lookup"><span data-stu-id="0cf68-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cf68-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cf68-140">JSON Representation</span></span>
<span data-ttu-id="0cf68-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cf68-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": 4.2
}
```




